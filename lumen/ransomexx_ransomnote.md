---
title: "RansomEXX (Defray777) Ransomware Note and Threat Actor Analysis"
description: "Comprehensive threat profile and verbatim ransom note samples for RansomEXX (Defray777), covering AES-256 ECB/RSA-4096 encryption, Linux and Windows targeting, Tor negotiation chat portals, and email channels."
author: "0xApollyon"
tags: [ransomexx, defray777, ransomware, aes-256-ecb, rsa-4096, threat-intelligence, tor-negotiation, dfir]
category: "Threat Intelligence"
keywords: ["RansomEXX", "Defray777", "ransom note", "threat intelligence", "cyberarkrules@gmail.com", "AES 256 ECB", "RSA 4096", "rnsm777cdsjrsdlbs4v5qoeppu3px6sb2igmh53jzrx7ipcrbjz5b2ad.onion", "double extortion"]
source_url: "https://abbadon.tech/lumen/ransomexx_ransomnote.html"
---

# RansomEXX (Defray777) Ransomware Note

> **Entity Summary:** RansomEXX (historically tracked as Defray777) is a sophisticated big-game hunting ransomware group operating since 2018. Renowned as one of the earliest ransomware families to develop specialized native Linux ELF binaries targeting VMware ESXi environments alongside standard Windows builds, RansomEXX implements hybrid AES-256 ECB and RSA-4096 encryption. The operators utilize unique victim-specific Tor negotiation portals (`rnsm777...onion`) and historical email contact points for extortion communications.

---

## Threat Actor Profile & Technical Metadata

| Attribute | Details |
| :--- | :--- |
| **Threat Actor** | RansomEXX (Defray777) |
| **Status** | Active |
| **Primary Encryption** | AES 256 ECB, RSA 4096 |
| **Target Architecture** | Windows, Linux / VMware ESXi |
| **Extortion Scheme** | Big Game Hunting Double Extortion (Confidential Data Theft & High-Impact Encryption) |
| **Negotiation Portal (Tor)**| `http://rnsm777cdsjrsdlbs4v5qoeppu3px6sb2igmh53jzrx7ipcrbjz5b2ad.onion/`<br>`http://jbdg4buq6jd7ed3rd6cynqtq5abttuekjnxqrqyvk4xam5i7ld33jvqd.onion/` |
| **Communication Email** | `cyberarkrules@gmail.com` |
| **Lumen Reference** | [Lumen Directory](https://abbadon.tech/lumen) |

---

## Ransom Note Samples

### Sample 1: Data Theft & Tor Chat Notice
```text
Attention: Your data has undergone encryption.
It is imperative that you abstain from any attempts to modify or rename the encrypted files,
as such actions could result in substantial data loss and decryption complications.

We have downloaded 134GB of your confidential data and we are ready yo publish it.

Access your personalized link to communicate with us about resolving this issue (make sure to use the Tor browser):
http://jbdg4buq6jd7ed3rd6cynqtq5abttuekjnxqrqyvk4xam5i7ld33jvqd.onion/[snip]/chat
```

### Sample 2: Targeted Incident Link Notice
```text
Hello!

Your data was encrypted.
Please don’t try to modify or rename any of encrypted files, because it can result in serious data loss and decryption failure.

Note that we've downloaded a lot of your files from [snip] and we are ready to publish it.
Contact us ASAP to prevent it.

Your personal link with full information regarding this accident (use Tor browser):
http://rnsm777cdsjrsdlbs4v5qoeppu3px6sb2igmh53jzrx7ipcrbjz5b2ad.onion/[snip]/
```

### Sample 3: Formatted String Notice
```text
Attention: Your data has undergone encryption.\nIt is imperative that you abstain from any attempts to modify or rename the encrypted files,
as such actions could result in substantial data loss and decryption complications.

Access your personalized link to communicate with us about resolving this issue (make sure to use the Tor browser):
http://jbdg4buq6jd7ed3rd6cynqtq5abttuekjnxqrqyvk4xam5i7ld33jvqd.onion/[snip]/chat
```

### Sample 4: Short Identifier Notice
```text
Hello [snip]!
Your files are ENCRYPTED.
Don't modify or rename them because it may cause decryption failure.
To get details about this accident download TOR browser and visit:
http://rnsm777cdsjrsdlbs4v5qoeppu3px6sb2igmh53jzrx7ipcrbjz5b2ad.onion/[snip]
```

### Sample 5: IT Department & Email Extortion Notice
```text
Greetings, [snip]!
Read this message CAREFULLY and contact someone from IT department.
Your files are securely ENCRYPTED.
No third party decryption software EXISTS.
MODIFICATION or RENAMING encrypted files may cause decryption failure.
You can send us an encrypted file (not greater than 400KB) and we will decrypt it FOR FREE,
so you have no doubts in possibility to restore all files from all affected systems ANY TIME.
Encrypted file SHOULD NOT contain sensitive information (technical, backups, databases, large documents).
The rest of data will be available after the PAYMENT.
Infrastructure rebuild will cost you MUCH more.
Contact us ONLY if you officially represent the whole affected network.
The ONLY attachments we accept are non archived encrypted files for test decryption.
Speak ENGLISH when contacting us.
Mail us: cyberarkrules@gmail.com
We kindly ask you not to use GMAIL, YAHOO or LIVE to contact us.
The PRICE depends on how quickly you do it.
```
