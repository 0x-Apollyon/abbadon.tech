---
title: "Money Message Ransomware Note and Threat Actor Analysis"
description: "Comprehensive threat profile and verbatim ransom note sample from the Money Message ransomware operation, covering their ChaCha20/ECDH cryptographic model, victim chat portal, and darknet leak site."
author: "0xApollyon"
tags: [moneymessage, money-message, ransomware, chacha20, ecdh, threat-intelligence, tor-negotiation, dfir]
category: "Threat Intelligence"
keywords: ["Money Message", "Money message ransomware", "blogvl7tjyjvsfthobttze52w36wwiz34hrfcmorgvdzb6hikucb7aqd.onion", "ransom note", "threat intelligence", "ChaCha20", "ECDH", "cyber extortion"]
source_url: "https://abbadon.tech/lumen/moneymessage_ransomnote.html"
---

# Money Message Ransomware Note

> **Entity Summary:** Money Message is a double-extortion ransomware syndicate discovered in March 2023, widely recognized for high-profile intrusions into PC hardware manufacturers and multinational enterprises. The threat actors utilize high-performance hybrid encryption combining ChaCha20 stream cipher with Elliptic Curve Diffie-Hellman (ECDH) key exchange. Victims are directed to a dedicated Tor chat application, with threats of releasing exfiltrated data on their public darknet blog if demands are ignored.

---

## Threat Actor Profile & Technical Metadata

| Attribute | Details |
| :--- | :--- |
| **Threat Actor** | Money Message ("Money message profitable organization") |
| **Status** | Active |
| **Primary Encryption** | ChaCha20, ECDH (Elliptic-Curve Cryptography) |
| **Target Architecture** | Windows, Linux / VMware ESXi |
| **Extortion Scheme** | Double Extortion (High-Volume Data Exfiltration & File Encryption) |
| **Leak Site (Tor)** | `http://blogvl7tjyjvsfthobttze52w36wwiz34hrfcmorgvdzb6hikucb7aqd.onion` |
| **Negotiation Portal (Tor)**| `http://clientcuworpelkdwecucgvfhp5uz5n7uohsnokndrlhm2zkntyg3had.onion/chat.php?chatId=[snip]` |
| **Lumen Reference** | [Lumen Directory](https://abbadon.tech/lumen) |

---

## Ransom Note Samples

### Sample 1: Standard Extortion & Negotiation Notice
```text
Your files was encrypted by "Money message" profitable organization and can't be accessed anymore. If you pay ransom, you will get a decryptor to decrypt them. Don't try to decrypt files yourself - in that case they will be damaged and unrecoverable. For further negotiations open this clientcuworpelkdwecucgvfhp5uz5n7uohsnokndrlhm2zkntyg3had.onion/chat.php?chatId=[snip] using tor browser https://www.torproject.org/download/ In case you refuse to pay, we will post the files we stole from your internal network, in our blog: blogvl7tjyjvsfthobttze52w36wwiz34hrfcmorgvdzb6hikucb7aqd.onion Encrypted files can't be decrypted without our decryption software.
```
