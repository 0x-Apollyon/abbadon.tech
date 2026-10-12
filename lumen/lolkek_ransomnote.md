---
title: "Bit (Lolkek / Globeimposter) Ransomware Note and Threat Actor Analysis"
description: "Analysis and verbatim ransom note samples from the Bit / Lolkek ransomware variant, associated with the Globeimposter ransomware family, including payment instructions and email contact channels."
author: "0xApollyon"
tags: [lolkek, globeimposter, bit-ransomware, ransomware, crypto-ransomware, threat-intelligence, dfir]
category: "Threat Intelligence"
keywords: ["Lolkek", "Bit Ransomware", "Globeimposter", "ransom note", "threat intelligence", "filessupport@cock.li", "sendmebtc@india.com", "bitcoin extortion"]
source_url: "https://abbadon.tech/lumen/lolkek_ransomnote.html"
---

# Bit (Lolkek / Globeimposter) Ransomware Note

> **Entity Summary:** Bit (also identified by victim file extensions `.lolkek` and `.bit`) is a ransomware lineage tied to the broader Globeimposter ransomware family. Characterized by opportunistic dissemination (often via compromised Remote Desktop Protocol (RDP) sessions or malicious spam attachments), this strain encrypts local and networked volumes and instructs victims to communicate via disposable email services (`cock.li`, `india.com`) or shortlink ticket systems to arrange fixed Bitcoin ransoms.

---

## Threat Actor Profile & Technical Metadata

| Attribute | Details |
| :--- | :--- |
| **Threat Actor** | Bit (Lolkek) (Globeimposter Family) |
| **Status** | Offline / Historical |
| **Primary Encryption** | RSA, AES-256 (Globeimposter cryptographic framework) |
| **Target Architecture** | Windows |
| **Extortion Scheme** | Single Extortion (Volume Encryption with Static BTC Demand) |
| **Email Contacts** | `filessupport@cock.li`<br>`sendmebtc@india.com`<br>`byd@india.com` |
| **Ticket / External Portals**| `hxxps://yip.su/2QstD5` |
| **Observed BTC Address** | `16G8L4oJs87e7kACZ6W4PNZLsXAkxxXsuWe` (1 BTC demand) |
| **Lumen Reference** | [Lumen Directory](https://abbadon.tech/lumen) |

---

## Ransom Note Samples

### Sample 1: Short Ticket Variant
```text
Attention!

 

All your files are encrypted

 

if you want to recover files write to email filessupport@cock.li

 

or create ticket here: hxxps://yip.su/2QstD5
```

### Sample 2: Detailed Payment & Exchange Instructions Variant
```text
Your files are encrypted!
All your important data has been encrypted.
To recover data you need decryptor.
To get the decryptor you should:
pay for decrypt:
site for buy bitcoin:
Buy 1 BTC on one of theses site:
1. localbitcoins.com
2. coinbase.com
3. xchange.cc


Bitcoin address to pay: 16G8L4oJs87e7kACZ6W4PNZLsXAkxxXsuWe
Send 1 BTC for decrypt. After the payment: Send screenshot of payment to sendmebtc@india.com, byd@india.com. In the letter include your personal ID (look at the beginning of this document). After you will receive a decryptor and instructions. Attention! No Payment = No decryption. You really get the decryptor after payment. Do not attempt to remove the program or run the anti-virus tools. Attempts to self-decrypting files will result in the loss of your data. Decoders other users are not compatible with your data, because each user’s unique encryption key.
```
