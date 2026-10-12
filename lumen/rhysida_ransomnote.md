---
title: "Rhysida Ransomware Note and Threat Actor Analysis"
description: "Comprehensive threat analysis and verbatim ransom note samples for Rhysida ransomware, detailing ChaCha20/RSA-4096 encryption, healthcare and education sector targeting, and darknet leak infrastructure."
author: "0xApollyon"
tags: [rhysida, ransomware, raas, chacha20, rsa-4096, threat-intelligence, tor-negotiation, dfir]
category: "Threat Intelligence"
keywords: ["Rhysida", "Rhysida ransomware", "rhysidafohrhyy2aszi7bm32tnjat5xri65fopcxkdfxhi4tidsg7cad.onion", "ransom note", "threat intelligence", "ChaCha20", "RSA 4096", "cyber extortion"]
source_url: "https://abbadon.tech/lumen/rhysida_ransomnote.html"
---

# Rhysida Ransomware Note

> **Entity Summary:** Rhysida is an aggressive Ransomware-as-a-Service (RaaS) operation that first emerged in May 2023. Gaining international notoriety for devastating attacks on healthcare organizations, government municipalities, and gaming and educational institutions, Rhysida postures in its ransom notices as a pseudo-benevolent "cybersecurity team". The malware utilizes hybrid ChaCha20 and RSA-4096 cryptography, forcing victims into darknet auction sites (`rhysidafoh...onion`) where stolen corporate data is auctioned to the highest bidder if ransoms are not settled.

---

## Threat Actor Profile & Technical Metadata

| Attribute | Details |
| :--- | :--- |
| **Threat Actor** | Rhysida |
| **Status** | Active |
| **Primary Encryption** | ChaCha20, RSA 4096 |
| **Target Architecture** | Windows, Linux / VMware ESXi |
| **Extortion Scheme** | Double Extortion (High-Impact Data Auctions & Enterprise Encryption) |
| **Leak Site / Portal (Tor)**| `http://rhysidafohrhyy2aszi7bm32tnjat5xri65fopcxkdfxhi4tidsg7cad.onion` |
| **Communication Emails** | `ChantellGrant@onionmail.org`<br>`LorriBuckridge@onionmail.org` |
| **Lumen Reference** | [Lumen Directory](https://abbadon.tech/lumen) |

---

## Ransom Note Samples

### Sample 1: Standard Darknet Portal Notice
```text
Critical Breach Detected - Immediate Response Required

Dear company,

This is an automated alert from cybersecurity team Rhysida. An unfortunate situation has arisen - your digital ecosystem has been compromised, and a substantial amount of confidential data has been exfiltrated from your network. The potential ramifications of this could be dire, including the sale, publication, or distribution of your data to competitors or media outlets. This could inflict significant reputational and financial damage.

However, this situation is not without a remedy.

Our team has developed a unique key, specifically designed to restore your digital security. This key represents the first and most crucial step in recovering from this situation. To utilize this key, visit our secure portal: rhysidafohrhyy2aszi7bm32tnjat5xri65fopcxkdfxhi4tidsg7cad.onion with your secret key [snip]

It's vital to note that any attempts to decrypt the encrypted files independently could lead to permanent data loss. We strongly advise against such actions.

Time is a critical factor in mitigating the impact of this breach. With each passing moment, the potential damage escalates. Your immediate action and full cooperation are required to navigate this scenario effectively.

Rest assured, our team is committed to guiding you through this process. The journey to resolution begins with the use of the unique key. Together, we can restore the security of your digital environment.

Best regards
```

### Sample 2: OnionMail Fallback Variant
```text
Dear company,


This is an automated alert from cybersecurity team Rhysida. An unfortunate
situation has arisen – your digital ecosystem has been compromised, and a
substantial amount of confidential data has been exfiltrated from your network.
The potential ramifications of this could be dire, including the sale, publication,
or distribution of your data to competitors or media outlets. This could inflict
significant reputational and financial damage.


However, this situation is not without a remedy.


Our team has developed a unique key, specifically designed to restore your
digital security. This key represents the first and most crucial step in
recovering from this situation. To utilize this key, visit our secure portal:
- with your
secret key - or write email:
ChantellGrant@onionmail.org LorriBuckridge@onionmail.org


It’s vital to note that any attempts to decrypt the encrypted files independently
could lead to permanent data loss. We strongly advise against such actions.


Time is a critical factor in mitigating the impact of this breach. With each
passing moment, the potential damage escalates. Your immediate action and
full cooperation are required to navigate this scenario effectively.


Rest assured, our team is committed to guiding you through this process. The
journey to resolution begins with the use of the unique key. Together, we can
restore the security of your digital environment.


Best regards
```
