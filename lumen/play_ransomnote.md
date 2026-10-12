---
title: "Play (PlayCrypt) Ransomware Note and Threat Actor Analysis"
description: "Comprehensive threat profile and verbatim ransom note samples for Play (PlayCrypt) ransomware, highlighting their distinctively concise ransom notes, AES-256 GCM encryption, and Tor leak portals."
author: "0xApollyon"
tags: [play, playcrypt, play-ransomware, ransomware, aes-256-gcm, rsa-2048, threat-intelligence, dfir]
category: "Threat Intelligence"
keywords: ["Play ransomware", "PlayCrypt", "mbrlkbtq5jonaqkurjwmxftytyn2ethqvbxfu4rgjbkkknndqwae6byd.onion", "k7kg3jqxang3wh7hnmaiokchk7qoebupfgoik6rha6mjpzwupwtj25yd.onion", "ransom note", "threat intelligence", "AES 256 GCM", "RSA 2048"]
source_url: "https://abbadon.tech/lumen/play_ransomnote.html"
---

# Play (PlayCrypt) Ransomware Note

> **Entity Summary:** Play (also identified by security analysts as PlayCrypt) is a prominent closed-loop cyber-extortion group active since June 2022. Renowned for impactful strikes against government agencies, municipal infrastructure, and critical supply chains, Play utilizes intermittent encryption with AES-256 GCM and RSA-2048. Their ransom notes are famously minimal—typically containing only the group moniker "PLAY", an email address (often hosted on GMX), and darknet leak portal URLs.

---

## Threat Actor Profile & Technical Metadata

| Attribute | Details |
| :--- | :--- |
| **Threat Actor** | Play (PlayCrypt) |
| **Status** | Active |
| **Primary Encryption** | AES 256 GCM, RSA 2048 (Intermittent Encryption) |
| **Target Architecture** | Windows, Linux / VMware ESXi |
| **Extortion Scheme** | Double Extortion (Confidential File Exfiltration & Disk Encryption) |
| **Leak Site (Tor)** | `mbrlkbtq5jonaqkurjwmxftytyn2ethqvbxfu4rgjbkkknndqwae6byd.onion`<br>`k7kg3jqxang3wh7hnmaiokchk7qoebupfgoik6rha6mjpzwupwtj25yd.onion` |
| **Communication Emails** | `teilightomemaucd@gmx.com`<br>`derdiarikucisv@gmx.de` |
| **Lumen Reference** | [Lumen Directory](https://abbadon.tech/lumen) |

---

## Ransom Note Samples

### Sample 1: Minimal Contact Notice
```text
PLAY
teilightomemaucd@gmx.com
```

### Sample 2: Multi-Onion Portal Notice
```text
PLAY
news portal, tor network links:
mbrlkbtq5jonaqkurjwmxftytyn2ethqvbxfu4rgjbkkknndqwae6byd.onion
k7kg3jqxang3wh7hnmaiokchk7qoebupfgoik6rha6mjpzwupwtj25yd.onion
derdiarikucisv@gmx.de
```
