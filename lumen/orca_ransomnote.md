---
title: "Orca Ransomware Note and Threat Actor Analysis"
description: "Threat profile and verbatim ransom note sample from the Orca ransomware variant, detailing encryption mechanisms (RC4, RSA-2048), Bitcoin extortion demands, and email communication channels."
author: "0xApollyon"
tags: [orca, orca-ransomware, ransomware, rc4, rsa-2048, threat-intelligence, dfir]
category: "Threat Intelligence"
keywords: ["Orca", "Orca ransomware", "GoldenSunMola", "ransom note", "threat intelligence", "RC4", "RSA 2048", "cyber extortion", "bitcoin ransom"]
source_url: "https://abbadon.tech/lumen/orca_ransomnote.html"
---

# Orca Ransomware Note

> **Entity Summary:** Orca is an extortionate ransomware strain detected in early 2023 that opportunistically targets enterprise Windows environments. Utilizing an encryption routine combining RC4 stream ciphers, Base64 encoding, and RSA-2048 public-key cryptography, Orca appends custom extensions to affected assets. The threat actors threaten data publication and operate primarily through disposable webmail addresses (`GoldenSunMola@aol.com`, `GoldenSunMola@cyberfear.com`), requiring ransom transactions in Bitcoin (BTC).

---

## Threat Actor Profile & Technical Metadata

| Attribute | Details |
| :--- | :--- |
| **Threat Actor** | Orca |
| **Status** | Active |
| **Primary Encryption** | RC4, BASE64, RSA 2048 |
| **Target Architecture** | Windows |
| **Extortion Scheme** | Double Extortion (Confidential Data Theft & File Encryption) |
| **Payment Method** | Bitcoin (BTC) |
| **Email Contacts** | `GoldenSunMola@aol.com`<br>`GoldenSunMola@cyberfear.com` |
| **Lumen Reference** | [Lumen Directory](https://abbadon.tech/lumen) |

---

## Ransom Note Samples

### Sample 1: Standard Extortion Notice
```text
YOUR FILES HAVE BEEN ENCRYPTED
Your ID to decrypt: -
Contact us: GoldenSunMola@aol.com | GoldenSunMola@cyberfear.com


Unfortunately for you, due to a serious vulnerability in IT security, you are vulnerable to attacks!
To decrypt files, you need to get a private key.
The only copy of the secret key that can be used to decrypt files is on a private server.
The server will destroy the key within 72h after the encryption is completed.
To save the key for a longer period, you can contact us and provide your ID!


In addition, we collect strictly confidential/personal data.
This data is also stored on a private server.
Your data will be deleted only after payment!
If you decide not to pay, we will publish your data to everyone or resellers.
So you can expect your data to become publicly available in the near future!


It's just a business and we only care about making a profit!
The only way to get your files back is to contact us for further instructions!
To establish a trust relationship, you can send 1 file for test decryption (no more than 5 MB)


Do not waste your time searching for other decryption methods - THERE ARE NONE, you will pay more for your time!
Every day the price of decryption increases!
Do not rename encrypted files.
Do not use third-party programs to decrypt files - they can only do harm!
After payment, you get a decoder (.exe), you only need to run it, and it will do everything by itself.
I only accept Bitcoins! You can learn how to buy them on the Internet.
```
