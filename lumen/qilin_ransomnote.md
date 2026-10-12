---
title: "Qilin (Agenda) Ransomware Note and Threat Actor Analysis"
description: "Comprehensive threat analysis and verbatim ransom note samples for Qilin (formerly Agenda) ransomware, detailing Go and Rust implementations, AES/ChaCha20 encryption, and Tor credential portals."
author: "0xApollyon"
tags: [qilin, agenda, ransomware, raas, golang, rust, chacha20, aes-256, rsa-4096, threat-intelligence, dfir]
category: "Threat Intelligence"
keywords: ["Qilin", "Agenda ransomware", "Qilin ransomware", "e3v6tjarcltwc4hdkn6fxnpkzq42ul7swf5cfqw6jzvic4577vxsxhid.onion", "ransom note", "threat intelligence", "Rust ransomware", "Go ransomware", "double extortion"]
source_url: "https://abbadon.tech/lumen/qilin_ransomnote.html"
---

# Qilin (Agenda) Ransomware Note

> **Entity Summary:** Qilin (originally observed in mid-2022 under the name Agenda) is an advanced Ransomware-as-a-Service (RaaS) syndicate operating across global healthcare, education, critical manufacturing, and technology sectors. Originally compiled in Golang and subsequently rewritten in Rust for enhanced evasion and execution speed, Qilin implements customizable encryption schemes using AES-256 or ChaCha20 paired with RSA-4096. Victims receive credentials to access an individualized Tor portal for chat and negotiation.

---

## Threat Actor Profile & Technical Metadata

| Attribute | Details |
| :--- | :--- |
| **Threat Actor** | Qilin (formerly Agenda) |
| **Status** | Active |
| **Primary Encryption** | AES 256, ChaCha20, RSA 4096 (Golang & Rust implementations) |
| **Target Architecture** | Windows, Linux / VMware ESXi |
| **Extortion Scheme** | Double Extortion (High-Volume Data Exfiltration & File Locking) |
| **Negotiation Portal (Tor)**| `http://wlh3dpptx2gt7nsxcor37a3kiyaiy6qwhdv7o6nl6iuniu5ycze5ydid.onion`<br>`http://e3v6tjarcltwc4hdkn6fxnpkzq42ul7swf5cfqw6jzvic4577vxsxhid.onion` |
| **Lumen Reference** | [Lumen Directory](https://abbadon.tech/lumen) |

---

## Ransom Note Samples

### Sample 1: Agenda Variant
```text
-- Agenda

Your network/system was encrypted.
Encrypted files have new extension.

-- Compromising and sensitive data

We have downloaded compromising and sensitive data from you system/network
If you refuse to communicate with us and we do not come to an agreementyour data will be published.
Data includes:
    - Employees personal dataCVsDLSSN.
    - Complete network map including credentials for local and remote services.
    - Financial information including clients databillsbudgetsannual reportsbank statements.
    - Complete datagrams/schemas/drawings for manufacturing in solidworks format
    - And more...

-- Warning

1) If you modify files - our decrypt software won't able to recover data
2) If you use third party software - you can damage/modify files (see item 1)
3) You need cipher key / our decrypt software to restore you files.
4) The police or authorities will not be able to help you get the cipher key. We encourage you to consider your decisions.

-- Recovery

1) Download tor browser: https://www.torproject.org/download/
2) Go to domain
3) Enter credentials


-- Credentials

Extension: DtMXQFOCos
Domain: wlh3dpptx2gt7nsxcor37a3kiyaiy6qwhdv7o6nl6iuniu5ycze5ydid.onion
login: [snip] 
password: [snip]
```

### Sample 2: Qilin Variant
```text
-- Qilin



Your network/system was encrypted.

Encrypted files have new extension.



-- Compromising and sensitive data



We have downloaded compromising and sensitive data from you system/network

If you refuse to communicate with us and we do not come to an agreement, your data will be published.

Data includes:

- Employees personal data, CVs, DL , SSN.

- Complete network map including credentials for local and remote services.

- Financial information including clients data, bills, budgets, annual reports, bank statements.

- Complete datagrams/schemas/drawings for manufacturing in solidworks format

- And more...



-- Warning



1) If you modify files - our decrypt software won't able to recover data

2) If you use third party software - you can damage/modify files (see item 1)

3) You need cipher key / our decrypt software to restore you files.

4) The police or authorities will not be able to help you get the cipher key. We encourage you to consider your decisions.



-- Recovery



1) Download tor browser: https://www.torproject.org/download/

2) Go to domain

3) Enter credentials-- Credentials

Extension: [snip]
Domain: e3v6tjarcltwc4hdkn6fxnpkzq42ul7swf5cfqw6jzvic4577vxsxhid.onion
login: [snip]
password:[snip]
```
