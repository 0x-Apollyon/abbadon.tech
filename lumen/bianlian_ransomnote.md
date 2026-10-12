---
title: "BianLian Ransomware - Ransom Note Sample & Threat Intelligence"
description: "Ransom note sample and threat analysis for the BianLian extortion operation, documenting AES-256 encryption, pure exfiltration pivot, I2P/Tor leak mirrors, and Tox communication channels."
author: "0xApollyon"
tags: [ransomware, bianlian, threat-intelligence, ransom-note, aes-256, tox, i2p, tor, the-lumen-register]
category: "Threat Intelligence"
keywords: ["BianLian ransomware", "BianLian ransom note", "BianLian threat actor", "The Lumen Register", "AES 256", "Tox messenger", "I2P leak site", "pure extortion"]
source_url: "https://abbadon.tech/lumen/bianlian_ransomnote.html"
---

# BianLian Ransom Note

> **Entity Summary:** BianLian is an active ransomware and data extortion group active since 2022. Initially employing AES-256 file encryption before pivoting primarily toward pure data theft extortion, BianLian targets healthcare, education, and professional services. Victims are directed to communicate via Tox messenger or onionmail, with stolen records hosted across Tor and I2P darknet mirrors.

## Threat Profile & Metadata

| Attribute | Details |
| :--- | :--- |
| **Threat Actor** | BianLian |
| **Status** | Active |
| **Known Encryption** | AES 256 |
| **Primary Communication** | Tox Messenger, Onionmail, Tor & I2P portals |
| **Onion Leak Portals** | `http://bianlianlbc5an4kgnay3opdemgcryg2kpfcbgczopmm3dnbz3uaunad.onion`, `http://bianlivemqbawcco4cx4a672k2fip3guyxudzurfqvdszafam3ofqgqd.onion` |
| **I2P Leak Site** | `http://epovhlzpj3grgld7vxr2mnk33dz5rdb4kdcp44f5r527rvhwhxna.b32.i2p` |
| **Tox IDs** | `A8AD0FD4C931CDAA1408D5A60CBF38CEDF46B41E19A8A55E4EF1F1848AF3416AE52D278D37DF`<br>`A4B3B0845DA242A64BF17E0DB4278EDF85855739667D3E2AE8B89D5439015F07E81D12D767FC` |
| **Contact Emails** | `deepmind@onionmail.org`, `swikipedia@onionmail.org`, `swikipedia.reserve@onionmail.org` |
| **Lumen Reference** | [bianlian_ransomnote.html](https://abbadon.tech/lumen/bianlian_ransomnote.html) |

---

## Ransom Note Samples

### Ransom Note

```text
Your network systems were attacked and encrypted. Contact us in order to restore your data. Don't make any changes in your file structure: touch no files, don't try to recover by yourself, that may lead to it's complete loss. To contact us you have to download "tox" messenger: https://qtox.github.io/ Add user with the following ID to get your instructions: A4B3B0845DA242A64BF17E0DB4278EDF85855739667D3E2AE8B89D5439015F07E81D12D767FC Alternative way: swikipedia@onionmail.org Your ID: [snip] You should know that we have been downloading data from your network for a significant time before the attack: financial, client, business, post, technical and personal files. In 10 days - it will be posted at our site http://bianlianlbc5an4kgnay3opdemgcryg2kpfcbgczopmm3dnbz3uaunad.onion / http://bianlivemqbawcco4cx4a672k2fip3guyxudzurfqvdszafam3ofqgqd.onion with links send to your clients, partners, competitors and news agencies, that will lead to a negative impact on your company: potential financial, business and reputational loses. ---!!!---
```
