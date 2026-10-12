---
title: "Malas (MalasLocker) Ransomware Note and Threat Actor Analysis"
description: "Analysis and verbatim ransom note sample from the Malas (MalasLocker) ransomware operation, showcasing their unconventional charity donation extortion model and age-tool encryption."
author: "0xApollyon"
tags: [malas, malaslocker, ransomware, age-encryption, charity-extortion, threat-intelligence, dfir]
category: "Threat Intelligence"
keywords: ["Malas", "MalasLocker", "somos malas podemos ser peores", "ransom note", "threat intelligence", "AGE encryption", "Zimbra vulnerability", "charity extortion"]
source_url: "https://abbadon.tech/lumen/malas_ransomnote.html"
---

# Malas (MalasLocker) Ransomware Note

> **Entity Summary:** Malas (also recognized as MalasLocker) is an atypical ransomware operation that gained notoriety in early 2023 primarily targeting Zimbra Collaboration servers. Unusually, instead of demanding cryptocurrency payments directly to their own wallets, Malas extorts organizations by requiring evidence of donations made to approved non-profit organizations or charitable foundations. Cryptographically, the operation leverages the modern `age` encryption utility (implementing X25519, ChaCha20-Poly1305, and AES standards).

---

## Threat Actor Profile & Technical Metadata

| Attribute | Details |
| :--- | :--- |
| **Threat Actor** | Malas (MalasLocker) |
| **Status** | Active |
| **Primary Encryption** | AES, X25519, ChaCha20-Poly1305 (via `age` encryption tool) |
| **Target Architecture** | Linux, Zimbra Collaboration suites, Windows |
| **Extortion Scheme** | Hacktivism / Ideological Charity Donation Extortion |
| **Communication Email** | `somos.malas.podemos.ser.peores@protonmail.com` |
| **Tor Fallback** | `http://blablabla.onion` *(template placeholder)* |
| **Cryptographic Block** | `-----BEGIN AGE ENCRYPTED FILE-----` |
| **Lumen Reference** | [Lumen Directory](https://abbadon.tech/lumen) |

---

## Ransom Note Samples

### Sample 1: Standard Extortion & Non-Profit Donation Notice
```text
Your files have been encrypted with AES military-grade encryption. Our data
recovery and security specialists can help you decrypt your files and secure
your server from hackers. Contact us and we'll provide a decrypter that will
safely and quickly restore your files. Any other attempts to recover your files
will be a waste of your time and money, and risk permanent data loss.  Your
files have been securely encrypted with AES, and the only way to decrypt is by
sending us the contents of the \"BEGIN AGE ENCRYPTED FILE\" block below, which
we can use to create a decrypter for you.

Unlike traditional ransomware groups, we're not asking you to send us money. We
just dislike corporations and economic inequality. We simply ask that you make a
donation to a non-profit that we approve of. It's a win-win, you can probably
get a tax deduction and good PR from your donation if you want.

Our email contact is somos.malas.podemos.ser.peores@protonmail.com
If you don't receive a reply within 24 hours, check your spam folder.

If you still haven't received a reply, use Tor Browser (https://www.torproject.org/download/) to visit:
http://blablabla.onion
there will be posted our current contact information


-----BEGIN AGE ENCRYPTED FILE-----
blablabla
-----END AGE ENCRYPTED FILE-----
```
