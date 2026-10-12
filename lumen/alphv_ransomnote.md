---
title: "AlphV (BlackCat) Ransomware - Ransom Note Samples & Threat Intelligence"
description: "Comprehensive ransom note samples and threat intelligence for the seized AlphV (BlackCat) ransomware operation, detailing Rust-based payloads, AES/ChaCha20 encryption, and Tor victim panels."
author: "0xApollyon"
tags: [ransomware, alphv, blackcat, threat-intelligence, ransom-note, rust, aes, chacha20, law-enforcement-seized, the-lumen-register]
category: "Threat Intelligence"
keywords: ["AlphV ransomware", "BlackCat ransomware", "AlphV ransom note", "BlackCat ransom note", "The Lumen Register", "AES encryption", "ChaCha20", "Rust ransomware", "law enforcement seizure"]
source_url: "https://abbadon.tech/lumen/alphv_ransomnote.html"
---

# AlphV (BlackCat) Ransom Note

> **Entity Summary:** AlphV (also known as BlackCat) was a notorious Ransomware-as-a-Service (RaaS) syndicate programmed in Rust that executed devastating double-extortion campaigns worldwide. The malware offered configurable encryption algorithms (AES or ChaCha20) and private Tor-based negotiation portals for each victim. The group's infrastructure was seized by international law enforcement operations led by the FBI.

## Threat Profile & Metadata

| Attribute | Details |
| :--- | :--- |
| **Threat Actor** | AlphV (BlackCat) |
| **Status** | Seized |
| **Known Encryption** | AES or ChaCha20 |
| **Implementation Language** | Rust |
| **Primary Communication** | Tor Hidden Service victim panels and Tox |
| **Seized Onion Leak Site** | `http://alphvmmm27o3abo3r2mlmjrpdmzle3rykajqc5xsj7j7ejksbpsa36ad.onion` |
| **Offline Onion Mirrors** | `http://vqifktlreqpudvulhbzmc5gocbeawl67uvs2pttswemdorbnhaddohyd.onion`, `http://sty5r4hhb5oihbq2mwevrofdiqbgesi66rvxr5sr573xgvtuvr4cs5yd.onion`, `http://xnsbsjciylsg23zfmrv6ocuyh7ha5zexeouchlr3zsi5suda4arpeyqd.onion` |
| **Tox ID** | `3488458145EB62D7D3947E3811234F4663D9B5AEEF6584AB08A2099A7F946664BBA2B0D30BFC` |
| **Lumen Reference** | [alphv_ransomnote.html](https://abbadon.tech/lumen/alphv_ransomnote.html) |

---

## Ransom Note Samples

### Ransomnote 1

```text
Data on Your network was exfiltrated and encrypted.

Modifying encrypted files will result in permanent data loss!

Get in touch with us ASAP to get an offer:
1. Download and install Tor Browser from https://www.torproject.org/
2. Access User Panel at http://msv7eaydbdue7x6hos2kzbtwgoi7xmtuddlqgniqghs3qc54wajudwad.onion/?access-key=[snip]
   THIS IS YOUR PRIVATE USER PANEL ADDRESS, DO NOT SHARE IT WITH ANYONE!



See also:
  Visit our Blog: http://alphvmmm27o3abo3r2mlmjrpdmzle3rykajqc5xsj7j7ejksbpsa36ad.onion
  Social Media: https://twitter.com/search?q=%23alphv
```

### Ransomnote 2

```text
Hello, [snip]

>> What happened?

Important files on your network was ENCRYPTED and now they have "${EXTENSION}" extension.
In order to recover your files you need to follow instructions below.

>> Sensitive Data

Sensitive data on your network was DOWNLOADED.
If you DON'T WANT your sensitive data to be PUBLISHED you have to act quickly.

Data includes:
- MICROS DATABASE, Accounting, Drawings
- Check Copies, Engineering, HR, Banking Information
- Payroll Scan, Sales and Marketing, Financia
- And more...

>> CAUTION

DO NOT MODIFY ENCRYPTED FILES YOURSELF.
DO NOT USE THIRD PARTY SOFTWARE TO RESTORE YOUR DATA.
YOU MAY DAMAGE YOUR FILES, IT WILL RESULT IN PERMANENT DATA LOSS.

>> What should I do next?

1) Download and install Tor Browser from: https://torproject.org/
2) Navigate to: http://d75itpgjjfe2ys2qivqplbvmw3yyx7o5e4ppt2esit2lluhngulz4hqd.onion/?access-key=[snip]
```

### Ransomnote 3

```text
>> What happened?

Important files on your network was ENCRYPTED and now they have "${EXTENSION}" extension.
In order to recover your files you need to follow instructions below.

>> Sensitive Data

Sensitive data on your system was DOWNLOADED.
If you DON'T WANT your sensitive data to be PUBLISHED you have to act quickly.

Data includes:
- Employees personal data, CVs, DL, SSN.
- Complete network map including credentials for local and remote services.
- Private financial information including: clients data, bills, budgets, annual reports, bank statements.
- Manufacturing documents including: datagrams, schemas, drawings in solidworks format
- And more...

Private URL: http://alphvmmm27o3abo3r2mlmjrpdmzle3rykajqc5xsj7j7ejksbpsa36ad.onion/[snip]


>> CAUTION

DO NOT MODIFY ENCRYPTED FILES YOURSELF.
DO NOT USE THIRD PARTY SOFTWARE TO RESTORE YOUR DATA.
YOU MAY DAMAGE YOUR FILES, IT WILL RESULT IN PERMANENT DATA LOSS.

>> What should I do next?

Follow these simple steps to get everything back to normal:
1) Download and install Tor Browser from: https://torproject.org/
2) Navigate to: http://xnsbsjciylsg23zfmrv6ocuyh7ha5zexeouchlr3zsi5suda4arpeyqd.onion/?access-key=[snip]
```

### Ransomnote 4

```text
>> Introduction

Important files on your system was ENCRYPTED and now they have have "${EXTENSION}" extension.
In order to recover your files you need to follow instructions below.

>> Sensitive Data

Sensitive data on your system was DOWNLOADED and it will be PUBLISHED if you refuse to cooperate.

Data includes:
- Employees personal data, CVs, DL, SSN.
- Complete network map including credentials for local and remote services.
- Financial information including clients data, bills, budgets, annual reports, bank statements.
- Complete datagrams/schemas/drawings for manufacturing in solidworks format
- And more...

Private preview is published here: http://alphvmmm27o3abo3r2mlmjrpdmzle3rykajqc5xsj7j7ejksbpsa36ad.onion/[snip]


>> CAUTION

DO NOT MODIFY FILES YOURSELF.
DO NOT USE THIRD PARTY SOFTWARE TO RESTORE YOUR DATA.
YOU MAY DAMAGE YOUR FILES, IT WILL RESULT IN PERMANENT DATA LOSS.
YOUR DATA IS STRONGLY ENCRYPTED, YOU CAN NOT DECRYPT IT WITHOUT CIPHER KEY.

>> Recovery procedure

Follow these simple steps to get in touch and recover your data:
1) Download and install Tor Browser from: https://torproject.org/
2) Navigate to: http://sty5r4hhb5oihbq2mwevrofdiqbgesi66rvxr5sr573xgvtuvr4cs5yd.onion/?access-key=${ACCESS_KEY}
```
