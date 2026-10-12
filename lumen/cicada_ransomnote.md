---
title: "Cicada 3301 Ransomware - Ransom Note Sample & Threat Intelligence"
description: "Ransom note sample and threat analysis for Cicada 3301 ransomware, documenting ChaCha20 file encryption, ESXi/Linux targeting, Rust payloads, and Tor extortion portals."
author: "0xApollyon"
tags: [ransomware, cicada-3301, threat-intelligence, ransom-note, chacha20, rust, esxi, tor, the-lumen-register]
category: "Threat Intelligence"
keywords: ["Cicada 3301 ransomware", "Cicada3301 ransom note", "Rust ransomware", "The Lumen Register", "ChaCha20", "ESXi ransomware", "cicadabv7vicyvgz5khl7v2x5yygcgow7ryy6yppwmxii4eoobdaztqd onion"]
source_url: "https://abbadon.tech/lumen/cicada_ransomnote.html"
---

# Cicada 3301 Ransom Note

> **Entity Summary:** Cicada 3301 is an active ransomware operation that surfaced in mid-2024, borrowing the name and iconography of the legendary internet cryptography puzzle. Developed in Rust, the payload shares architectural similarities with BlackCat/ALPHV and specifically targets Windows and VMware ESXi environments using ChaCha20 encryption alongside terabyte-scale data exfiltration.

## Threat Profile & Metadata

| Attribute | Details |
| :--- | :--- |
| **Threat Actor** | Cicada 3301 |
| **Status** | Active |
| **Known Encryption** | ChaCha20 |
| **Payload Architecture** | Rust cross-platform (Windows & Linux/ESXi) |
| **Primary Communication** | Tor Hidden Service leak and chat portal |
| **Onion Leak Site** | `http://cicadabv7vicyvgz5khl7v2x5yygcgow7ryy6yppwmxii4eoobdaztqd.onion` |
| **Lumen Reference** | [cicada_ransomnote.html](https://abbadon.tech/lumen/cicada_ransomnote.html) |

---

## Ransom Note Samples

### Ransom Note

```text
*************************************
*** Welcome to Cicada3301 ***
*************************************


** What Happened? **
----------------------------------------------
Your computers and servers are encrypted, your backups are deleted.
We use strong encryption algorithms, so you won't be able to decrypt your data.
You can recover everything by purchasing a special data recovery program from us.
This program will restore your entire network.

 

** Data Leak **
----------------------------------------------
We have downloaded more than 1500 GB of your company data.
Contact us, or we will be forced to publish all your data on the Internet
and send it to all regulatory authorities in your country, as well as to your customers, partners, and competitors.


We are ready to:
- Provide you with proof that the data has been stolen;
- Delete all stolen data;
- Help you rebuild your infrastructure and prevent similar attacks in the future;


** What Guarantees? **
----------------------------------------------
Our reputation is of paramount importance to us.
Failure to fulfill our obligations means not working with you, which is against our interests.
Rest assured, our decryption tools have been thoroughly tested and are guaranteed to unlock your data.
Should any problems arise, we are here to support you. As a goodwill gesture,
we are willing to decrypt one file for free.


** How to Contact us? **
----------------------------------------------
Using TOR Browser:
1) You can download and install the TOR browser from this site: hxxps://torproject.org/
2) Open our website:
-


WARNING: DO NOT MODIFY or attempt to restore any files on your own. This can lead to their permanent loss.
```
