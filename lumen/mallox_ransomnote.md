---
title: "Mallox (TargetCompany) Ransomware Note and Threat Actor Analysis"
description: "Comprehensive threat analysis and verbatim ransom note samples from the Mallox ransomware operation (TargetCompany / FARGO), detailing encryption methods, Tor portals, and communication channels."
author: "0xApollyon"
tags: [mallox, targetcompany, fargo, tohnichi, ransomware, chacha20, aes-128, threat-intelligence, dfir]
category: "Threat Intelligence"
keywords: ["Mallox", "TargetCompany", "FARGO ransomware", "mallox resurrection", "ransom note", "threat intelligence", "ChaCha20", "AES-128 CTR", "wtyafjyhwqrgo4a45wdvvwhen3cx4euie73qvlhkhvlrexljoyuklaad.onion"]
source_url: "https://abbadon.tech/lumen/mallox_ransomnote.html"
---

# Mallox (TargetCompany) Ransomware Note

> **Entity Summary:** Mallox (also tracked as TargetCompany, FARGO, and Tohnichi) is a financially motivated ransomware group active since mid-2021. The threat actors routinely infiltrate corporate environments via brute-forced or exposed Microsoft SQL (MS-SQL) servers and vulnerable public-facing web applications. Utilizing hybrid ChaCha20 and AES-128 CTR encryption schemes, Mallox exfiltrates sensitive tables and demands ransoms via dedicated Tor negotiation portals and OnionMail communication channels.

---

## Threat Actor Profile & Technical Metadata

| Attribute | Details |
| :--- | :--- |
| **Threat Actor** | Mallox (TargetCompany / FARGO / Tohnichi) |
| **Status** | Active |
| **Primary Encryption** | ChaCha20, AES-128 CTR |
| **Target Architecture** | Windows, MS-SQL Server environments |
| **Extortion Scheme** | Double Extortion (Database Exfiltration & Endpoint Encryption) |
| **Leak Site (Tor)** | `http://wtyafjyhwqrgo4a45wdvvwhen3cx4euie73qvlhkhvlrexljoyuklaad.onion` |
| **Negotiation Portal (Tor)**| `http://wtyafjyhwqrgo4a45wdvvwhen3cx4euie73qvlhkhvlrexljoyuklaad.onion/mallox/privateSignin` |
| **Communication Emails** | `mallox@onionmail.org`<br>`mallox.resurrection@onionmail.org`<br>`mallox.israel@mailfence.com`<br>`mallox@tutanota.com` |
| **Lumen Reference** | [Lumen Directory](https://abbadon.tech/lumen) |

---

## Ransom Note Samples

### Sample 1: Standard Tor Negotiation & Data Leak Notice
```text
Hello

Your files are encrypted and can not be used
We have downloaded your confidential data and are ready to publish it on our blog
To return your files in work condition you need decryption tool
Follow the instructions to decrypt all your data

Do not try to change or restore files yourself, this will break them
If you want, on our site you can decrypt one file for free. Free test decryption allowed only for not valuable file with size less than 3MB

How to get decryption tool:
1) Download and install TOR browser by this link: https://www.torproject.org/download/
2) If TOR blocked in your country and you can't access to the link then use any VPN software
3) Run TOR browser and open the site: wtyafjyhwqrgo4a45wdvvwhen3cx4euie73qvlhkhvlrexljoyuklaad.onion/mallox/privateSignin
4) Copy your private ID in the input field. Your Private key: [snip]
5) You will see payment information and we can make free test decryption here
6)After payment, you will receive a tool for decrypting files, and we will delete the data that was taken from you

Our blog of leaked companies:
wtyafjyhwqrgo4a45wdvvwhen3cx4euie73qvlhkhvlrexljoyuklaad.onion

If you are unable to contact us through the site, then you can email us: mallox@onionmail.org
Waiting for a response via mail can be several days. Do not use it if you have not tried contacting through the site. of government supervision agencies, your competitors and clients. --------------------------------------------------------------------------------------------------
```

### Sample 2: Resurrection Variant
```text
Hello

Your files are encrypted and can not be used
To return your files in work condition you need decryption tool
Follow the instructions to decrypt all your data

Do not try to change or restore files yourself, this will break them
If you want, on our site you can decrypt one file for free. Free test decryption allowed only for not valuable file with size less than 3MB

How to get decryption tool:
1) Download and install TOR browser by this link: https://www.torproject.org/download/
2) If TOR blocked in your country and you can't access to the link then use any VPN software
3) Run TOR browser and open the site: wtyafjyhwqrgo4a45wdvvwhen3cx4euie73qvlhkhvlrexljoyuklaad.onion/mallox/privateSignin
4) Copy your private ID in the input field. Your Private key: [snip]
5) You will see payment information and we can make free test decryption here

Our blog of leaked companies:
wtyafjyhwqrgo4a45wdvvwhen3cx4euie73qvlhkhvlrexljoyuklaad.onion

If you are unable to contact us through the site, then you can email us: mallox.resurrection@onionmail.org
Waiting for a response via mail can be several days. Do not use it if you have not tried contacting through the site.  
```

### Sample 3: Early / Email-Direct Variant
```text
YOUR FILES ARE ENCRYPTED !!!

TO DECRYPT, FOLLOW THE INSTRUCTIONS:

To recover data you need decrypt tool.

To get the decrypt tool you should:

1.In the letter include your personal ID! Send me this ID in your first email to me!
2.We can give you free test for decrypt few files (NOT VALUE) and assign the price for decryption all files!
3.After we send you instruction how to pay for decrypt tool and after payment you will receive a decryption tool!
4.We can decrypt few files in quality the evidence that we have the decoder.


CONTACT US:
mallox.israel@mailfence.com
mallox@tutanota.com

YOUR PERSONAL ID: -
```
