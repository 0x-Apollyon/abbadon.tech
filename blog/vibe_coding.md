---
title: "Basic security in the age of vibecoding"
description: "Vibe coding lets you generate code with LLMs instead of learning to code. While powerful, it's easy to mess up and leave your B2B SaaS app vulnerable. Here's a checklist of 10 security fundamentals to keep your webapp from getting obliterated."
author: "0xApollyon"
date: 2025-03-19
tags: [infosec, ai, vibe-coding, web-security, application-security, saas]
category: "Infosec"
keywords: ["vibe coding security", "web application security checklist", "API key exposure", "XSS", "IDOR", "CORS misconfiguration", "Firebase security rules", "S3 bucket security", "SQL injection", "DDoS protection", "rate limiting"]
source_url: "https://abbadon.tech/blog/vibe_coding.html"
---

# Basic security in the age of vibecoding

## So what is vibecoding?

Vibe coding, the art of prompting LLMs to generate code for you instead of learning to code. While it does empower many people to build whatever they want and increases productivity by orders of magnitude, it is very easy to mess up your code and your B2B SaaS app, which is supposed to make you a gazillion dollars, is obliterated by randoms on the internet.

![I'm under attack](./vibe_coding_imgs/im_under_attack.png)

It is easy to point and laugh at the tech bros who claim to be earning the big bucks without spending a single second actually writing code, but its better if they are helped because we all were noobs once (though some of the tech bros have been noobs for too long ngl).

So this is a basic checklist of stuff you should do so your webapp doesnt go down the drain coz of basic vulnerabilities. While it will not make your vibecoded project "unhackable", it would sure make it a lot, lot safer.

---

## 1: No API keys on the frontend, ever

Do not put any API keys, client secrets, auth tokens, private keys and ANYTHING of similar nature on the frontend. Even billion dollar VC firms are guilty of this crime (im looking at you a16z). This is like the cardinal sin of infosec. If you are putting API keys on the frontend, you are inherently exposing them to anyone who uses your webapp. And no, base64 encoding them , client side encrypting them or using a minifier doesnt fix the issue.

![Fired meme](./vibe_coding_imgs/fired.png)

Threat actors can and will use exposed API keys to make requests as legitimate users. They will abuse it till they can, and if its a paid API you can say goodbye to them sweet credits. Worst case scenario, all your user data gets published on breachforums and your reputation is obliterated.

![BreachForums listing](./vibe_coding_imgs/breachforums.png)

If your webapp is using external APIs, route all requests through your backend, which handles authentication properly. Use short lived OAuth flows or some other form of authentication on your frontend and also monitor the API usage to detect sus traffic. Implement periodic key rotation if possible.

---

## 2: Cross site scripting

Cross site scripting occurs when your website takes input and displays it as literal HTML code, allowing attackers to execute arbitrary JS. This is usually disastrous, as now anyone can steal cookies or modify page content to phish credentials (or add UFOs to your game), there are an infinite number of attacks.

There are three main types of XSS attacks—stored, reflected, and DOM. Out of these, stored XSS, which is persistent, is the one that impacts most vibecoded projects. One rule of thumb to keep in mind is, never trust the frontend. Always sanitize the input, be it usernames, text, profile pictures, forum posts or stuff of similar nature.

Use filters like React's inbuilt JSX filtering, Djangos escape(), libraries like DOMPurify or whatever it is in the framework you are using. Also implement a content security policy (CSP) which prohibits scripts from random external sources. To prevent cookies from being stolen, use the HTTP only flag.

---

## 3: Actually paid content

Vibe coding is big with the tech bros as stated earlier, so its obvious that most vibe coded projects are trying to sell you something. But the thing is people dont like paying for stuff, and they will access your content or software for free if they can. If you do have content which is behind a paywall, make sure the paywall is enforced on the backend, and its not just some hidden API endpoint, some obscure URL parameter, a frontend only block or something.

A surprising number of developers assume that just because their content or features are behind a UI-based paywall, users will respect it. Security through obscurity is a very flawed approach and it will eventually go tits up, so will your project if you are following it.

![Fog of war meme](./vibe_coding_imgs/fog_of_war.png)

Heres a short list of ineffective "paywalling" methods:

- JS only frontend paywalls – A simple frontend check like `if (user.isPaid) { showContent() }` that can be bypassed with a single line in the browser console.
- Hidden API Endpoints – An API that serves premium content but has no authentication, meaning anyone who finds the URL can access it freely.
- Soft Restrictions – Using CSS to "blur" text or disable buttons while still loading the full content in the page source.

If you are using any of these methods, you arent using a paywall but instead a honor system. And well, the internet has no honor.

![Enemies meme](./vibe_coding_imgs/enemies.png)

To actually enforce a paywall, use backend verification. Ensure that all premium content and features are served only after a verified backend check. Every request must be authenticated, and the users subscription status should be validated before serving premium content. Also assume that people WILL try to bypass your paywall. Regularly audit your authentication flows and logs to detect unauthorized access.

---

## 4: IDORs

IDOR, which is an acronym for "Insecure Direct Object Reference" is a vulnerability that has catastrophic consequences if exploited (it is also my "favourite" vulnerability). When exploited, IDOR can lead to data breaches, unauthorized account takeovers, and full system compromise with minimal effort.

Say you have an API endpoint which accepts a user id and deletes the users account.

```
POST /delete
Body: { "user_id": 123 }
```

Now if you dont check if the ID of the user in the request is actually the user, a threat actor can simply change the user id and deletes someone elses account.

```
POST /delete
Body: { "user_id": 124 }
```

Combine this with a for loop iterating through all user ids and suddenly your "next facebook" has zero users, or maybe it had zero users in the first place.

Big multibillion dollar companies (Facebook, Twitter/X, Pandabuy) aswell as government agencies have falled victim to this vulnerability.

![Pandabuy breach](./vibe_coding_imgs/pandabuy.png)

To prevent your "next facebook" from being added to this list, ensure the logged-in user owns the object being accessed before performing any action (read, update, delete). Also track and alert on suspicious object access patterns, such as a single user requesting multiple user IDs in quick succession.

---

## 5: CORS

CORS, which is an acronym for Cross-Origin Resource Sharing is a built in security mechanism in modern browsers which blocks cross origin requests by default (SOP: Same origin policy). By default, if a web page on example.com tries to fetch data from api.example.com, the browser blocks the request unless api.example.com explicitly allows it via CORS headers. There are two main CORS headers:

- ACAO (Access Control Allow Origin): This controls which domains are allowed to access the resources.
- ACAC (Access Control Allow Credentials): This controls whether cookies and credentials (such as session tokens) can be sent with cross-origin requests.

(There are two others, ACAH for allowed headers and ACAM for allowed methods but they are pretty much irrelevant here)

Now, you might be tempted to set ACAO header to * to allow all your domains to access the resources. WRONG. NOT ONLY IS THIS LAZY (laziness is a "virtue" in a society - Doreen Ford on Fox News, Jan 25, 2022), IT MAKES YOUR APPLICATION INSECURE.

![Fox News interview](./vibe_coding_imgs/fox_news.png)

Setting Access-Control-Allow-Origin: * means any website, anywhere, can make requests to your API. This allows for attacks such as session hijacking. So to fix this, only allow trusted domains and subdomains in ACAO and ACAC, pretty easy.

Also time to insert a shameless plug, I have worked on a small utility YA-CORS to scan for common CORS misconfigurations. You can find it [here.](https://github.com/0x-Apollyon/YA-CORS)

---

## 6: Firebase on fire (This is also applicable to Supabase and other similar services)

Many SaaS projects, especially those without a dedicated backend, use services like Firebase for authentication and data storage (firestore, real time db). If improperly configured, anyone can access these databases and read, write stuff to them.

This has been a recurring vulnerability, especially with startups (chattr.ai, Arc Browser). These are just a few examples. Many more SaaS startups and apps have been caught leaking private user data due to bad Firebase/Supabase configs.

The root of the problem is default public access. By default, Firebase Realtime Database and Firestore allow public read/write access until rules are manually set. Below is a very common and very insecure security rule.

```json
{
  "rules": {
    ".read": true,
    ".write": true
  }
}
```

This means anyone on the internet can read all your data and modify or delete your database (reset user passwords, inject fake content and god knows what). Supabase is slightly better with Row Level Security (RLS), but if disabled, the database behaves like an open book for anyone with the API URL.

To fix this vulnerability, modify firestore rules to allow access only to authenticated users. For Supabase, do not disable (enable it if its disabled) Row Level Security (RLS) and write secure policies. This is very basic advice, read [this](https://firebase.google.com/support/guides/security-checklist) and [this](https://firebase.google.com/docs/rules/insecure-rules) for firebase. For supabase, read [this](https://supabase.com/docs/guides/database/postgres/row-level-security).

---

## 7: Leaky s3 buckets

Just like Firebase, many vibecoded projects also make use of s3 for storage, and it too is very easy to mess up and just like CORS vulnerabilities, the problems usually happen due to laziness and/or ignorance. The first, and the most common vulnerability which I have come across, is sensitive data in public, unsecure s3 buckets. Like many other vulnerabilities I have covered, even big corpporates (Twilio, Ford, Netflix) struggle with this.

![Netflix S3 leak](./vibe_coding_imgs/netflix_s3.png)

A threat actor can not only read from insecure buckets, but can also modify them. This can allow them to introduce malicious content, deface your webapp or even hold your files for ransom (Scattered Spider). Threat actors also love utilizing vulnerable s3 buckets as a way to exfiltrate data from their other operations without beind detected.

![S3 bucket attack diagram](./vibe_coding_imgs/s3.png)

To fix this issue, make sure your buckets are private by default, allow access only to your app by using bucket policies (or specific users/roles). Read [this](https://docs.aws.amazon.com/AmazonS3/latest/userguide/security-best-practices.html) for more info.

---

## 8: Ratelimits and anti bot measures

If people can automate abuse on your app, they will. Whether its for financial gain, competitive advantage, or just for the lulz, attackers (or even regular users) will spam your endpoints, scrape your data, and abuse your services if you dont put proper ratelimiting and anti bot features in place. While there is no way you can stop 100% of the bots, you can take some steps to stop the vast majority of them.

Implement rate limits on API endpoints, especially the ones you think might be targetted by a threat actor. You can use IP based ratelimits or user based ratelimits, whichever suits your usecase. For login, signups, and sensitive actions, use reCAPTCHA or hCaptcha to block bots. Aside from all this make sure to monitor logs for suspicious traffic spikes.

![CAPTCHA example](./vibe_coding_imgs/captcha.png)

---

## 9: DoS attacks

Denial of service attacks, or its elder brother, distributed denial of service (DDoS) attacks are some of the most common attacks that any webapp has to face. The barrier to entry is in the ground, and anyone, be it a basement dwelling nerd or a 12yo edgy child can launch. Also DDoS for hire services also exist, so best believe, if someone wants to DDoS your webapp, they will.

![DDoS illustration](./vibe_coding_imgs/ddos.png)

If you arent prepared for an attack like this, you can very easily run up a cloud bill comparable to the GDP of a third world country.

![AWS bill meme](./vibe_coding_imgs/aws.png)

There are many types of DDoS attacks, here I categorise the releavant ones into two categories

Type 1: Just a massive spray of traffic, not very interesting if im being honest. Can be mitigated using a DDoS protection service like Cloudflare, AWS Shield, Akamai, and similar services that filter out malicious traffic before it reaches your server.

Type 2: Application layer attacks, these spam your webapp with queries which are resource intensive and your webapp dies a death by a thousand cuts. These are often trickier to deal with compared to just a massive spray of traffic. To prevent these types of attacks, implement rate limiting on resource intensive API endpoints or alternatively use services like Cloudflare WAF, AWS WAF, and fastly to detect and block known patterns of such attacks.

![Cloudflare protection](./vibe_coding_imgs/cloudflare.png)

---

## 10: SQL and NoSQL injections

While this doesnt impact vibe coders as much as the other vulnerabilities, primarily because vibe coders are too dumb and lazy to use a proper SQL or NoSQL database. SQL injections have been here for decades and are still a menace, while NoSQL injections is the zoomer version impacting NoSQL databases. If you do use a SQL or NoSQL database, and you don't sanitize inputs, you're opening the gates to disaster. As previously stated, never trust the frontend. SQL injection happens when malicious SQL code makes its way into your database queries, usually through unsanitized user inputs.

![SQL injection comic](./vibe_coding_imgs/sqlinjection.png)

Example: Read the code given below, see if you can find how an attacker can exploit it.

```python
import mysql.connector
from flask import request, Flask

app = Flask(__name__)
db = mysql.connector.connect(user="root", password="password", database="users")

@app.route("/login", methods=["POST"])
def login():
    username = request.form["username"]
    password = request.form["password"]

    cursor = db.cursor()
    query = f"SELECT * FROM users WHERE username = '{username}' AND password = '{password}'"
    cursor.execute(query)

    if cursor.fetchone():
        return "Login successful"
    else:
        return "Invalid credentials"
```

NoSQL is basically the same, but impacts NoSQL databases such as Mongo. Example: This time, find the NoSQL injection -

```python
from flask import Flask, request
from pymongo import MongoClient

app = Flask(__name__)
client = MongoClient("mongodb://localhost:27017/")
db = client["usersDB"]
users_collection = db["users"]

@app.route("/login", methods=["POST"])
def login():
    username = request.json["username"]
    password = request.json["password"]

    user = users_collection.find_one({"username": username, "password": password})
    if user:
        return "Login successful"
    else:
        return "Invalid credentials"
```

To fix most SQL and NoSQL injection vulnerabilities, sanitize user input before passing it through and use parametrized queries so the database treats user inputs as values, not SQL code, preventing injections.

---

## Conclusion

So, thats it. Those were the 10 commandments of security in the era of vibecoders. As stated earlier, they will not make your app unhackable, but they will surely make it more safe. I hope this helps you secure your webapp, and not go insane fighting threat actors. Have fun vibecoding!!!

HEY!!! YOU MADE IT TO THE END. HERE IS A CAT PICTURE FOR YOU

![Blicky the cat](./vibe_coding_imgs/blicky.png)