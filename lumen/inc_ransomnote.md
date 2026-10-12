---
title: "INC Ransom Ransomware Note and Threat Actor Analysis"
description: "Comprehensive threat analysis and verbatim ransom note samples from the INC Ransom ransomware group, detailing extortion methods, encryption standards, and Tor portal communications."
author: "0xApollyon"
tags: [inc-ransom, ransomware, extortion, threat-intelligence, tor-negotiation, double-extortion, dfir]
category: "Threat Intelligence"
keywords: ["INC Ransom", "INC Ransomware", "inc pays", "inc blog", "ransom note", "threat intelligence", "RSA 2048", "cyber extortion"]
source_url: "https://abbadon.tech/lumen/inc_ransomnote.html"
---

# INC Ransom Ransomware Note

> **Entity Summary:** INC Ransom is a prominent double-extortion ransomware and data extortion group active since mid-2023. The syndicate targets enterprise and critical infrastructure organizations worldwide across healthcare, education, government, and commercial sectors. Their tactics involve exfiltrating terabytes of corporate records prior to network-wide encryption using RSA-2048 algorithms, threatening public disclosure via dedicated Tor and clearweb leak sites (`incapt[.]su`).

---

## Threat Actor Profile & Technical Metadata

| Attribute | Details |
| :--- | :--- |
| **Threat Actor** | INC Ransom (Inc. Ransomware) |
| **Status** | Active |
| **Primary Encryption** | RSA 2048 |
| **Target Architecture** | Windows, Linux / VMware ESXi |
| **Extortion Scheme** | Double Extortion (Data Exfiltration & Volume Encryption), Pure Extortion Attacks |
| **Leak Site (Tor)** | `http://incblog6qu4y4mm4zvw5nrmue6qbwtgjsxpw6b7ixzssu36tsajldoad.onion/`<br>`http://incblog7vmuq7rktic73r4ha4j757m3ptym37tyvifzp2roedyyzzxid.onion/` |
| **Negotiation Portal (Tor)**| `http://incpaykabjqc2mtdxq6c23nqh4x6m5dkps5fr6vgdkgzp5njssx6qkid.onion/`<br>`http://incpaysp74dphcbjyvg2eepxnl3tkgt5mq5vd4tnjusoissz342bdnad.onion/` |
| **Clearweb Mirrors** | `http://incapt.su/` |
| **Lumen Reference** | [Lumen Directory](https://abbadon.tech/lumen) |

---

## Ransom Note Samples

### Sample 1: HTML Embedded Notice
```html
<html> <head> <title>Inc. Ransomware</title> </head> <body style="width: 100%; height: 100%; display: flex; flex-direction: column; justify-content: center; align-items: center; overflow: auto;"> <div
style="max-width: 500px; "> <h1 style="text-align: center;">Inc. Ransomware</h1> <div> <p>We have hacked you and downloaded all confidential data of your company and its clients. It can be spread out to people and media.
Your reputation will be ruined. Do not hesitate and save your business.</p> <p>Please, contact us via:</p> <p style="margin-left: 32px;">http://incpaysp74dphcbjyvg2eepxnl3tkgt5mq5vd4tnjusoissz342bdnad.onion/</p>
<div> <div> <p>Your personal ID:</p> <p style="margin-left: 32px;">[snip]</p> <div> <div> <p>We're the ones who can quickly recover your systems with no losses. Do not try to devalue
our tool - nothing will come of it.</p> <p>Starting from now, you have 72 hours to contact us if you don't want your sensitive data being published in our blog:</p> <p style="margin-left: 32px;">http://incblog7vmuq7rktic73r4ha4j757m3ptym37tyvifzp2roedyyzzxid.onion/</p>
<p>You should be informed, in our business reputation - is a basic condition of the success.</p> <div> <div> <p>Inc provides a deal. After successfull negotiations you will be provided:</p> <ol>
<li>Decryption assistance;</li> <li>Initial access;</li> <li>How to secure your network;</li> <li>Evidence of deletion of internal documents.</li> </ol> <div> </div>
</body> </html>
```

### Sample 2: Text Notice with Deal Guarantees
```text
Inc. Ransomware

We have hacked you and downloaded all confidential data of your company and its clients.
It can be spread out to people and media. Your reputation will be ruined. 
Do not hesitate and save your business.

Please, contact us via:
	http://incpaysp74dphcbjyvg2eepxnl3tkgt5mq5vd4tnjusoissz342bdnad.onion/
	
Your personal ID:
	[snip]
	
We're the ones who can quickly recover your systems with no losses. Do not try to devalue our tool - nothing will come of it.

Starting from now, you have 72 hours to contact us if you don't want your sensitive data being published in our blog:

	http://incblog7vmuq7rktic73r4ha4j757m3ptym37tyvifzp2roedyyzzxid.onion/
	
You should be informed, in our business reputation - is a basic condition of the success.

Inc provides a deal. After successfull negotiations you will be provided:

	1. Decryption assistance;
	2. Initial access;
	3. How to secure your network;
	4. Evidence of deletion of internal documents;
	5. Guarantees not to attack you in the future.
```

### Sample 3: Text Notice with Tor Instructions
```text
Inc. Ransomware

We have hacked you and downloaded all confidential data of your company and its clients.
It can be spread out to people and media. Your reputation will be ruined. 
Do not hesitate and save your business.

Please, contact us via:
	http://incpaysp74dphcbjyvg2eepxnl3tkgt5mq5vd4tnjusoissz342bdnad.onion/
	
Your personal ID:
	[snip]
	
We're the ones who can quickly recover your systems with no losses. Do not try to devalue our tool - nothing will come of it.

Starting from now, you have 72 hours to contact us if you don't want your sensitive data being published in our blog:
	http://incblog7vmuq7rktic73r4ha4j757m3ptym37tyvifzp2roedyyzzxid.onion/
	
You should be informed, in our business reputation - is a basic condition of the success.

Inc provides a deal. After successfull negotiations you will be provided:
	1. Decryption assistance;
	2. Initial access;
	3. How to secure your network;
	4. Evidence of deletion of internal documents;
	5. Guarantees not to attack you in the future.
	
Instruction how to get to chat page:
	1. Download TOR Browser from official website (https://www.torproject.org/download/);
	2. Install TOR Browser and open it;
	3. Copy chat link and press enter;
	4. On the page you will need to register your account using your personal ID;
	5. Use this ID and your password to get chat page again.
```

### Sample 4: In-Depth Ransom Notice & Psychological Coercion
```text
~~~~ INC Ransom ~~~~

-----> Your data is stolen and encrypted.
If you don't pay the ransom, the data will be published on our TOR darknet sites.
The sooner you pay the ransom, the sooner your company will be safe.

Tor Browser Link:
	http://incblog6qu4y4mm4zvw5nrmue6qbwtgjsxpw6b7ixzssu36tsajldoad.onion/
	http://incblog7vmuq7rktic73r4ha4j757m3ptym37tyvifzp2roedyyzzxid.onion/

Link for normal browser:
	http://incapt.su/
	
-----> What guarantees are that we won't fool you?
We are not a politically motivated group and we want nothing more than money.
If you pay, we will provide you with decryption software and destroy the stolen data.
After you pay the ransom, you will quickly restore your systems and make even more money.
Treat this situation simply as a paid training for your system administrators, because it is due to your corporate network not being properly configured that we were able to attack you.
Our pentest services should be paid just like you pay the salaries of your system administrators. Get over it and pay for it.
If we don't give you a decryptor or delete your data after you pay, no one will pay us in the future.
You can get more information about us on Twitter https://twitter.com/hashtag/incransom?f=live

-----> You need to contact us on TOR darknet sites with your personal ID
Download and install Tor Browser https://www.torproject.org/
Write to the chat room and wait for an answer, we'll guarantee a response from you.
Sometimes you will have to wait some time for our reply, this is because we have a lot of work and we attack tens of companies around the world.

Tor Browser Link for chat:
	http://incpaykabjqc2mtdxq6c23nqh4x6m5dkps5fr6vgdkgzp5njssx6qkid.onion/

Your personal ID:
	[snip]

-----> Warning! Don't delete or modify encrypted files, it will lead to problems with decryption of files!
-----> Don't go to the police or the FBI for help. They won't help you.
The police will try to prohibit you from paying the ransom in any way.
The first thing they will tell you is that there's no guarantee to decrypt your files and remove stolen files.
This is not true, we can do a test decryption before paying and your data will be guaranteed to be removed because it's a matter of our reputation.
Paying the ransom to us is much cheaper and more profitable than paying fines and legal fees.
The police and the FBI don't care what losses you suffer as a result of our attack, and we'll help you get rid of all your problems for a modest sum of money.
If you're worried that someone will trace your bank transfers, you can easily buy cryptocurrency for cash, thus leaving no digital trail that someone from your company paid our ransom.
The police and FBI won't be able to stop lawsuits from your customers for leaking personal and private information.
The police and FBI won't protect you from repeated attacks. 

-----> Don't go to recovery companies!
They are essentially just middlemen who will make money off you and cheat you.
We are well aware of cases where recovery companies tell you that the ransom price is $5M dollars, but in fact they secretly negotiate with us for $1M.
If you approached us directly without intermediaries you would pay several times less.

-----> For those who have cyber insurance against ransomware attacks.
Insurance companies require you to keep your insurance information secret.
In most cases, we find this information and download it.

-----> If you do not pay the ransom, we will attack your company again in the future.
```

### Sample 5: Direct Notification / Extortion Email
```text
Greetings!
We inform you that the INC ransomware team hacked into your corporate network and downloaded more than a terabyte of confidential information.
As proof, we have attached some of the downloaded files to the email.
We know the attitude of your country's legislation in the field of cybersecurity, and in order not to give the incident loud publicity, we did not encrypt your network and sent mail only to management and official mail. We can settle this amicably.
To find out how to solve the situation in which you find yourself, you need to log into the chat to communicate:

Paste this link - http://incpaysp74dphcbjyvg2eepxnl3tkgt5mq5vd4tnjusoissz342bdnad.onion
Use this ID - [snip] - to create chat account
Install TOR Browser to get access to our chat room - https://www.torproject.org/download/

If you do not get in touch within 48 hours, your information will be published on our blog - http://incapt.su/blog/leaks .
And we will inform the major media about the incident.
```
