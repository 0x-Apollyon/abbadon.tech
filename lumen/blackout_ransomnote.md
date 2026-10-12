---
title: "Blackout Ransomware - Ransom Note Sample & Threat Intelligence"
description: "Ransom note sample and threat intelligence for Blackout ransomware, detailing AES-256 encryption, faux 'open-source license' disclaimer tactics, and mail2tor communication channels."
author: "0xApollyon"
tags: [ransomware, blackout, threat-intelligence, ransom-note, aes-256, mail2tor, telegram, the-lumen-register]
category: "Threat Intelligence"
keywords: ["Blackout ransomware", "Blackout ransom note", "Blackout decryptor", "The Lumen Register", "AES 256", "blackzd derpymail", "blackoutsupport mai12tor", "blackout_supp"]
source_url: "https://abbadon.tech/lumen/blackout_ransomnote.html"
---

# Blackout Ransom Note

> **Entity Summary:** Blackout is an active ransomware strain utilizing AES-256 symmetric encryption to lock Windows files. Notably, the threat actors include a deceptive pseudo-legal "license agreement" in their ransom instructions, claiming the malware is experimental open-source penetration testing software. The group routes victims through clearnet and mail2tor darknet email addresses and Tox messenger.

## Threat Profile & Metadata

| Attribute | Details |
| :--- | :--- |
| **Threat Actor** | Blackout |
| **Status** | Active |
| **Known Encryption** | AES 256 |
| **Primary Communication** | Tor Hidden Service, Telegram, Tox, Email |
| **Onion Site** | `http://black3gnkizshuynieigw6ejgpblb53mpasftzd6pydqpmq2vn2xf6yd.onion` |
| **Telegram Account** | [t.me/blackout_supp](https://t.me/blackout_supp) |
| **Tox ID** | `36A73D90C66948D9268BDC4174A40E0064C43F10A35AEAA9DD74B3A14EF5654872D5DC67FC14` |
| **Contact Emails** | `blackoutsupport@mai12tor.com`, `blackzd@derpymail.org`, `blackzd@xmail.net`, `blackzd@safe-mail.net`, `decrypted8@bigmir.net`, `tyspalento@bigmir.net`, `mitoplent@safe-mail.net` |
| **Lumen Reference** | [blackout_ransomnote.html](https://abbadon.tech/lumen/blackout_ransomnote.html) |

---

## Ransom Note Samples

### Ransom Note

```text
Your files have been encrypted ransomware!
Your personal Id:
ZiaDE*****UOY2E
LICENSE AGREEMENT
the Blackout Ransomware is a free open source software.
The program is designed to test the protection of OS Windows against ransomware.
The developer of this software is not responsible for any damage caused by the program.
The program is experimental and the entire responsibility for use lies with the user.
HOW TO USE:
To decrypt your files, you need the program blackout_decryptor.exe
If you do not have it, write to email: blackzd@derpymail.org or blackzd@xmail.net
In the letter, send your personal id and two small encrypted files for trial decryption.
If you dont get answer from blackzd@derpymail.org or blackzd@xmail.net in 72 hours,
you need to install tor browser, you can download it here:
https://www.torproject.org/download/download.html.en
After installation, open the tor browser to website:
http://mail2tor2zyjdctd.onion/register.php
Register on the site a new email address and write to us with his letter to our address:
blackoutsupport@mai12tor.com
NN:506358115267996
```
