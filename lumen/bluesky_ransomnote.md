---
title: "Bluesky Ransomware - Ransom Note Sample & Threat Intelligence"
description: "Ransom note sample and threat intelligence for the Bluesky ransomware family, documenting RC4 stream cipher encryption, Conti-derived loader tactics, and Tor recovery portals."
author: "0xApollyon"
tags: [ransomware, bluesky, threat-intelligence, ransom-note, rc4, tor, the-lumen-register]
category: "Threat Intelligence"
keywords: ["Bluesky ransomware", "Bluesky ransom note", "Bluesky decryptor", "The Lumen Register", "RC4 encryption", "ccpyeuptrlatb2piua4ukhnhi7lrxgerrcrj4p2b5uhbzqm2xgdjaqid onion"]
source_url: "https://abbadon.tech/lumen/bluesky_ransomnote.html"
---

# Bluesky Ransom Note

> **Entity Summary:** Bluesky is an active ransomware strain discovered in mid-2022 that exhibits code overlap with Conti ransomware loaders. Bluesky employs RC4 stream cipher encryption for rapid file locking, delivers multi-threaded payload execution, and directs victims to an interactive Tor negotiation portal using individual recovery identifiers.

## Threat Profile & Metadata

| Attribute | Details |
| :--- | :--- |
| **Threat Actor** | Bluesky |
| **Status** | Active |
| **Known Encryption** | RC4 |
| **Primary Communication** | Tor Hidden Service recovery portal |
| **Onion Recovery Portal** | `http://ccpyeuptrlatb2piua4ukhnhi7lrxgerrcrj4p2b5uhbzqm2xgdjaqid.onion` |
| **Lumen Reference** | [bluesky_ransomnote.html](https://abbadon.tech/lumen/bluesky_ransomnote.html) |

---

## Ransom Note Samples

### Ransom Note

```text
<<< B L U E S K Y >>> YOUR IMPORTANT FILES, DOCUMENTS, PHOTOS, VIDEOS, DATABASES HAVE BEEN ENCRYPTED! The only way to decrypt and restore your files is with our private key and program. Any attempts to restore your files manually will damage your files. To restore your files follow these instructions: -------------------------------------------------------------- 1. Download and install "Tor Browser" from https://torproject.org/ 2. Run "Tor Browser" 3. In the tor browser open website: http://ccpyeuptrlatb2piua4ukhnhi7lrxgerrcrj4p2b5uhbzqm2xgdjaqid.onion 4. On the website enter your recovery id: RECOVERY ID: [snip] 5. Follow the instructions --------------------------------------------------------------
```
