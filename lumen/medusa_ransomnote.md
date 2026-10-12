---
title: "Medusa Ransomware Note and Threat Actor Analysis"
description: "Comprehensive threat intelligence and verbatim ransom note analysis of the Medusa ransomware operation, covering encryption algorithms, OSINT extortion tactics, and darknet communications."
author: "0xApollyon"
tags: [medusa, ransomware, double-extortion, osint, aes-256, rsa-2048, threat-intelligence, dfir]
category: "Threat Intelligence"
keywords: ["Medusa ransomware", "Medusa decryptor", "medusaxko7jxtrojdkxo66j7ck4q5tgktf7uqsqyfry4ebnxlcbkccyd.onion", "ransom note", "threat intelligence", "AES 256", "RSA 2048", "Tox chat", "cyber extortion"]
source_url: "https://abbadon.tech/lumen/medusa_ransomnote.html"
---

# Medusa Ransomware Note

> **Entity Summary:** Medusa is an aggressive ransomware and cyber-extortion operation that surged in early 2023. Not to be confused with MedusaLocker, Medusa employs hybrid AES-256 and RSA-2048 encryption alongside active public-shaming campaigns. The group operates a dedicated "Medusa Blog" leak site on the Tor network and leverages dedicated OSINT, Telegram, and social media channels to aggressively amplify pressure on victimized corporate executives.

---

## Threat Actor Profile & Technical Metadata

| Attribute | Details |
| :--- | :--- |
| **Threat Actor** | Medusa |
| **Status** | Active |
| **Primary Encryption** | AES 256, RSA 2048 |
| **Target Architecture** | Windows, Linux / VMware ESXi |
| **Extortion Scheme** | Double Extortion (Full Network Exfiltration & File Encryption), Social Media Doxxing |
| **Leak Site (Tor)** | `http://medusaxko7jxtrojdkxo66j7ck4q5tgktf7uqsqyfry4ebnxlcbkccyd.onion/` |
| **Negotiation Portal (Tor)**| `http://medusakxxtp3uo7vusntvubnytaph4d3amxivbggl3hnhpk2nmus34yd.onion/` |
| **Tox ID** | `4AE245548F2A225882951FB14E9BF87EE01A0C10AE159B99D1EA62620D91A372205227254A9F` |
| **Support Email** | `medusa.support@onionmail.org` |
| **Lumen Reference** | [Lumen Directory](https://abbadon.tech/lumen) |

---

## Ransom Note Samples

### Sample 1: Standard Medusa Notice with ASCII Header
```text
$$\      $$\ $$$$$$$$\ $$$$$$$\  $$\   $$\  $$$$$$\   $$$$$$\  
$$$\    $$$ |$$  _____|$$  __$$\ $$ |  $$ |$$  __$$\ $$  __$$\ 
$$$$\  $$$$ |$$ |      $$ |  $$ |$$ |  $$ |$$ /  \__|$$ /  $$ |
$$\$$\$$ $$ |$$$$$\    $$ |  $$ |$$ |  $$ |\$$$$$$\  $$$$$$$$ |
$$ \$$$  $$ |$$  __|   $$ |  $$ |$$ |  $$ | \____$$\ $$  __$$ |
$$ |\$  /$$ |$$ |      $$ |  $$ |$$ |  $$ |$$\   $$ |$$ |  $$ |
$$ | \_/ $$ |$$$$$$$$\ $$$$$$$  |\$$$$$$  |\$$$$$$  |$$ |  $$ |
\__|     \__|\________|\_______/  \______/  \______/ \__|  \__|
-----------------------------[ Hello, [snip] !!! ]--------------------------

WHAT HAPPEND?
------------------------------------------------------------
1. We have PENETRATE your network and COPIED data.
* We have penetrated entire network including backup system and researched all about your data.
* And we have extracted all of your networks including sub offices and your service clients networks valuable data and copied them to private cloud storage.

2. We have ENCRYPTED some your files.
While you are reading this message, it means you found your files and data has been ENCRYPTED by world's strongest ransomware.
We have access to all of your sub offices and client service networks but didn't lock them all for your brand and privacy.
We can solve this issue sliently and smoothly without 3rd parties and we decided lock only some of your main network only.
But don't worry, we can restore everything to the original without harming your business.

There is only one possible way to get back your systems and business - CONTACT us via LIVE CHAT and pay for the special 
MEDUSA DECRYPTOR and DECRYPTION KEYs, Data deletion, Keep silent in media.
This MEDUSA DECRYPTOR will restore your entire network, This will take less than 1 business day.


WHAT GUARANTEES?
---------------------------------------------------------------
We can post your data to the public and send emails to your customers.
We have professional OSINTs and media team for leak data to telegram, facebook, twitter channels and top news websites. Have a look about us on twitter.

You can suffer significant problems due disastrous consequences, leading to loss of valuable intellectual property and other sensitive information, 
 costly incident response efforts, information misuse/abuse, loss of customer trust, brand and reputational damage, legal and regulatory issues.
After paying for the data breach and decryption, we guarantee that your data will never be leaked and this is also for our reputation.

YOU should be AWARE!
---------------------------------------------------------------
If you're not in main chile office, inform your supervisors and stay calm!
We will speak only with an authorized person. It can be the CEO, top management, etc.
In case you are not such a person - DON'T CONTACT US! Your decisions and action can result in serious harm to your company!


If you do not contact us within 3 days, We will start publish your case to our official blog and everybody will start notice your incident!
If you do not contact us within 5 days, We will start publish your case and leak video on all social channels and send emails to your customers!
--------------------[ Official blog tor address ]--------------------
Using TOR Browser(https://www.torproject.org/download/):

http://medusaxko7jxtrojdkxo66j7ck4q5tgktf7uqsqyfry4ebnxlcbkccyd.onion/


CONTACT US!
----------------------[ Your company live chat address ]---------------------------
Using TOR Browser(https://www.torproject.org/download/):

http://medusakxxtp3uo7vusntvubnytaph4d3amxivbggl3hnhpk2nmus34yd.onion/[snip]

Or Use Tox Chat Program(https://qtox.github.io/)
Add user with our tox ID and wait 24h : 4AE245548F2A225882951FB14E9BF87EE01A0C10AE159B99D1EA62620D91A372205227254A9F

Our support email: ( medusa.support@onionmail.org )

Company identification hash:
[snip]
```
