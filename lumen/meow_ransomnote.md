---
title: "Meow Leaks (Meow Ransomware) Note and Threat Actor Analysis"
description: "Threat profile and verbatim ransom note sample from the Meow Leaks ransomware operation, detailing communication handles across Telegram, secure email, and ChaCha20/RSA-4096 encryption."
author: "0xApollyon"
tags: [meow-leaks, meow-ransomware, ransomware, chacha20, rsa-4096, threat-intelligence, dfir]
category: "Threat Intelligence"
keywords: ["Meow Leaks", "Meow ransomware", "meowcorp2022", "meowcorp", "ransom note", "threat intelligence", "ChaCha20", "RSA 4096", "Telegram extortion"]
source_url: "https://abbadon.tech/lumen/meow_ransomnote.html"
---

# Meow Leaks (Meow Ransomware) Note

> **Entity Summary:** Meow Leaks (also known as Meow ransomware, linked to Conti-based source code forks) is an opportunistic ransomware and extortion operation that began appearing in late 2022. Identified by the signature `.MEOW` extension appended to locked victim assets, the group utilizes hybrid ChaCha20 and RSA-4096 encryption. Meow relies primarily on direct messaging platforms such as Telegram and disposable email services (`proton.me`, `onionmail.org`, `msgsafe.io`, `aol.com`) for ransom negotiation.

---

## Threat Actor Profile & Technical Metadata

| Attribute | Details |
| :--- | :--- |
| **Threat Actor** | Meow Leaks (Meow Ransomware) |
| **Status** | Active |
| **Primary Encryption** | ChaCha20, RSA 4096 |
| **Target Architecture** | Windows, Linux |
| **Extortion Scheme** | Double Extortion (Data Theft & Volume Encryption) |
| **Telegram Contacts** | `@meowcorp2022`<br>`@meowcorp123` |
| **Email Contacts** | `meowcorp2022@aol.com`<br>`meowcorp2022@proton.me`<br>`meowcorp@msgsafe.io`<br>`meowcorp@onionmail.org` |
| **Lumen Reference** | [Lumen Directory](https://abbadon.tech/lumen) |

---

## Ransom Note Samples

### Sample 1: Standard Meow Notice
```text
MEOW! MEOW! MEOW!  

Your files has been encrypted!

Need decrypt?  Write to e-mail:

meowcorp2022@aol.com

meowcorp2022@proton.me

meowcorp@msgsafe.io

meowcorp@onionmail.org

or Telegram:

@meowcorp2022

@meowcorp123

Uniq ID: -
```
