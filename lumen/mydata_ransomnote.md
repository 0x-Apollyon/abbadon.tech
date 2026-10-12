---
title: "Mydata (AlphaLocker) Ransomware Note and Threat Actor Analysis"
description: "Comprehensive threat analysis and verbatim ransom note samples for Mydata / AlphaLocker ransomware, featuring RSA-2048/AES-256 encryption, Tox communication, and Tor leak site infrastructure."
author: "0xApollyon"
tags: [mydata, alphalocker, alpha-ransomware, ransomware, rsa-2048, aes-256, threat-intelligence, tox-chat, tor-negotiation, dfir]
category: "Threat Intelligence"
keywords: ["Mydata", "AlphaLocker", "Alpha ransomware", "mydatae2d63il5oaxxangwnid5loq2qmtsol2ozr6vtb7yfm5ypzo6id.onion", "ransom note", "threat intelligence", "RSA 2048", "AES 256", "Tox chat"]
source_url: "https://abbadon.tech/lumen/mydata_ransomnote.html"
---

# Mydata (AlphaLocker) Ransomware Note

> **Entity Summary:** Mydata (operating under the moniker Alpha Locker / Alpha Ransomware) is a targeted double-extortion ransomware actor that surfaced in early 2023. Deploying hybrid RSA-2048 and AES-256 cryptographic standards across victim networks, the group pairs encrypted local files with confidential data exfiltration. Alpha Locker operates a dedicated Tor leak repository (`mydatae2d63il5...onion`) and coordinates direct ransom negotiations through decentralized Tox messenger instances and Tor ticket portals.

---

## Threat Actor Profile & Technical Metadata

| Attribute | Details |
| :--- | :--- |
| **Threat Actor** | Mydata (Alpha Locker / Alpha Ransomware) |
| **Status** | Active |
| **Primary Encryption** | RSA 2048, AES 256 |
| **Target Architecture** | Windows |
| **Extortion Scheme** | Double Extortion (Confidential Data Exfiltration & File Locking) |
| **Leak Site (Tor)** | `http://mydatae2d63il5oaxxangwnid5loq2qmtsol2ozr6vtb7yfm5ypzo6id.onion/blog` |
| **Negotiation Portal (Tor)**| `http://mydatae2d63il5oaxxangwnid5loq2qmtsol2ozr6vtb7yfm5ypzo6id.onion` |
| **Tox ID** | `98D120C9033653042E290627914B890A3291013F7377A976A028051C52440C71487D5F14DDA2` |
| **Lumen Reference** | [Lumen Directory](https://abbadon.tech/lumen) |

---

## Ransom Note Samples

### Sample 1: Alpha Locker Tox Messenger Variant
```text
Hello from Alpha Locker.
Your data have been stolen and encrypted.
Don't try to RECOVER, DELETE or MODIFY any files, this will make it impossible to restore.

We will help you in restoring your system, also decrypt several files for free.

You can contact us only via TOX messenger, download and install Tox client from: https://tox.chat/download.html
Add a friend with our TOX ID.

Our TOX ID: 98D120C9033653042E290627914B890A3291013F7377A976A028051C52440C71487D5F14DDA2
```

### Sample 2: Alpha Ransomware Tor Portal Variant
```text
            -=-=-=- Alpha ransomware -=-=-=-
   -=- Visit our blog: mydatae2d63il5oaxxangwnid5loq2qmtsol2ozr6vtb7yfm5ypzo6id.onion/blog -=-

-=- Your data have been stolen and encrypted -=-
-=- You won't be able to decrypt them without our help -=-
-=- Dont try to RECOVER, DELETE or MODIFY any files, this will make it impossible to restore -=-
-=- We will help you in restoring your system, also decrypt several files for free -=-

-=- Contact us for price and get decryption software -=-
Note that this server is available via Tor browser only Follow the instructions to open the link:
mydatae2d63il5oaxxangwnid5loq2qmtsol2ozr6vtb7yfm5ypzo6id.onion
1. Type the address "https://www.torproject.org" in your Internet browser. It opens the Tor site.  
2. Press "Download Tor", then press "Download Tor Browser", install and run it.
3. Now you have Tor browser. In the Tor Browser open mydatae2d63il5oaxxangwnid5loq2qmtsol2ozr6vtb7yfm5ypzo6id.onion
4. Copy your personal decryption key and paste it in the window that appears, enter the captcha and click the button submit.
5. Start a chat and follow the further instructions.

-----------------
Your personal decryption key:
[snip]
```
