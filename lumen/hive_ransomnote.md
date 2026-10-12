---
title: "Hive Ransomware - Ransom Note Samples & Threat Intelligence"
description: "Ransom note samples and threat intelligence for the seized Hive ransomware syndicate, documenting Go and Rust payloads, healthcare sector attacks, and Tor customer negotiation panels."
author: "0xApollyon"
tags: [ransomware, hive, threat-intelligence, ransom-note, golang, rust, law-enforcement-seized, tor, the-lumen-register]
category: "Threat Intelligence"
keywords: ["Hive ransomware", "Hive ransom note", "Hive decryptor", "The Lumen Register", "hiveleakdbtnp76ulyhi52eag6c6tyc3xw7ez7iqy6wc34gd2nekazyd onion", "FBI seizure Hive", "hivecust6vhekztbqgdnkks64ucehqacge3dij3gyrrpdp57zoq3ooqd onion"]
source_url: "https://abbadon.tech/lumen/hive_ransomnote.html"
---

# Hive Ransom Note

> **Entity Summary:** Hive was one of the most prolific and aggressive Ransomware-as-a-Service (RaaS) operations, heavily targeting hospitals, healthcare providers, and critical infrastructure globally. Initially developed in Go and later rewritten in Rust (Hive v5), the operation used in-memory key generation and victim-specific `*.key` files. In January 2023, the FBI and international law enforcement seized Hive's servers, darknet infrastructure, and decryption keys.

## Threat Profile & Metadata

| Attribute | Details |
| :--- | :--- |
| **Threat Actor** | Hive |
| **Status** | Seized |
| **Known Encryption** | ChaCha20-Poly1305, RSA / Custom (Historical) |
| **Codebase Versions** | Go (v1-v4), Rust (v5) |
| **Primary Communication** | Tor Hidden Service "sales department" portals |
| **Seized Onion Leak Site** | `http://hiveleakdbtnp76ulyhi52eag6c6tyc3xw7ez7iqy6wc34gd2nekazyd.onion` |
| **Seized Victim Portal** | `http://hivecust6vhekztbqgdnkks64ucehqacge3dij3gyrrpdp57zoq3ooqd.onion` |
| **Seized API Endpoint** | `http://hiveapi4nyabjdfz2hxdsr7otrcv6zq6m4rk5i2w7j64lrtny4b7vjad.onion` |
| **Lumen Reference** | [hive_ransomnote.html](https://abbadon.tech/lumen/hive_ransomnote.html) |

---

## Ransom Note Samples

### Ransomnote 1

```text
Your network has been breached and all data were encrypted.
Personal data, financial reports and important documents are ready to disclose.

To decrypt all the data and to prevent exfiltrated files to be disclosed at 
http://hiveleakdbtnp76ulyhi52eag6c6tyc3xw7ez7iqy6wc34gd2nekazyd.onion/
you will need to purchase our decryption software.

Please contact our sales department at:

   http://hivecust6vhekztbqgdnkks64ucehqacge3dij3gyrrpdp57zoq3ooqd.onion/

      Login:    [snip]
      Password: [snip]

To get an access to .onion websites download and install Tor Browser at:
   https://www.torproject.org/ (Tor Browser is not related to us)


Follow the guidelines below to avoid losing your data:

 - Do not delete or reinstall VMs. There will be nothing to decrypt.
 - Do not modify, rename or delete *.key files. Your data will be 
   undecryptable.
 - Do not modify or rename encrypted files. You will lose them.
 - Do not report to the Police, FBI, etc. They don't care about your business.
   They simply won't allow you to pay. As a result you will lose everything.
 - Do not hire a recovery company. They can't decrypt without the key. 
   They also don't care about your business. They believe that they are 
   good negotiators, but it is not. They usually fail. So speak for yourself.
 - Do not reject to purchase. Exfiltrated files will be publicly disclosed.
```

### Ransomnote 2

```text
Your network has been breached and all data were encrypted.
Personal data, financial reports and important documents are ready to disclose.

To decrypt all the data and to prevent exfiltrated files to be disclosed at 
http://hiveleakdbtnp76ulyhi52eag6c6tyc3xw7ez7iqy6wc34gd2nekazyd.onion/
you will need to purchase our decryption software.

Please contact our sales department at:

   http://hivecust6vhekztbqgdnkks64ucehqacge3dij3gyrrpdp57zoq3ooqd.onion/
  
      Login:    [snip]
      Password: [snip]

To get an access to .onion websites download and install Tor Browser at:
   https://www.torproject.org/ (Tor Browser is not related to us)


Follow the guidelines below to avoid losing your data:

 - Do not modify, rename or delete *.key.rrumj files. Your data will be 
   undecryptable.
 - Do not modify or rename encrypted files. You will lose them.
 - Do not report to the Police, FBI, etc. They don't care about your business.
   They simply won't allow you to pay. As a result you will lose everything.
 - Do not hire a recovery company. They can't decrypt without the key. 
   They also don't care about your business. They believe that they are 
   good negotiators, but it is not. They usually fail. So speak for yourself.
 - Do not reject to purchase. Exfiltrated files will be publicly disclosed.
```
