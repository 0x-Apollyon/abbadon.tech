---
title: "Trinity Ransomware Note and Threat Actor Analysis"
description: "Comprehensive threat analysis and verbatim ransom note sample from the Trinity ransomware operation, detailing their modern XChaCha20 and XSalsa20-Poly1305 / Curve25519 cryptography, OnionMail contacts, and double-extortion tactics."
author: "0xApollyon"
tags: [trinity, trinity-ransomware, ransomware, xchacha20, xsalsa20poly1305, curve25519, threat-intelligence, dfir]
category: "Threat Intelligence"
keywords: ["Trinity", "Trinity ransomware", "wehaveyourdata@onionmail.org", "ransom note", "threat intelligence", "XChaCha20", "XSalsa20-Poly1305", "Curve 25519", "cyber extortion"]
source_url: "https://abbadon.tech/lumen/trinity_ransomnote.html"
---

# Trinity Ransomware Note

> **Entity Summary:** Trinity is an advanced double-extortion ransomware threat discovered in mid-2024. Targeting critical healthcare providers and commercial institutions worldwide, Trinity employs state-of-the-art cryptographic primitives including XChaCha20 stream ciphers and XSalsa20-Poly1305 authenticated encryption backed by Curve25519 key exchange. Victims face a strict 24-hour response deadline backed by threats of darknet sales to commercial competitors and public doxxing via OnionMail and Tor-based portals.

---

## Threat Actor Profile & Technical Metadata

| Attribute | Details |
| :--- | :--- |
| **Threat Actor** | Trinity |
| **Status** | Active |
| **Primary Encryption** | XChaCha20, XSalsa20-Poly1305 with Curve 25519 |
| **Target Architecture** | Windows, Linux |
| **Extortion Scheme** | Double Extortion (Database Exfiltration & Advanced Authenticated Encryption) |
| **Communication Email** | `wehaveyourdata@onionmail.org` |
| **Negotiation Portal (Tor)**| `[Tor portal link embedded per target]` |
| **Lumen Reference** | [Lumen Directory](https://abbadon.tech/lumen) |

---

## Ransom Note Samples

### Sample 1: Standard Extortion & OnionMail Fallback Notice
```text
We downloaded to our servers and encrypted all your databases and personal information!


to contact us


download TOR


hxxps://www.torproject.org/download/


follow this link ********


follow the instructions on the website

 

if you're having trouble with TOR


e-mail wehaveyourdata@onionmail.org


IMPORTANT INFORMATION!


If you do not write to us within 24 hours, we will start publishing and selling your data on the darknet on hacker sites and offer the information to your competitors


Guarantee:If we don't provide you with a decryptor or delete your data after you pay,no one will pay us in the future. We value our reputation.


Guarantee key:To prove that the decryption key exists, we can test the file (not the database and backup) for free.


Do not try to decrypt your data using third party software, it may cause permanent data loss.


Don't go to recovery companies - they are essentially just middlemen.Decryption of your files with the help of third parties may cause increased price (they add their fee to our) we're the only ones who have the decryption keys.
```
