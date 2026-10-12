---
title: "Moses Staff Ransomware / Wiper Note and Threat Actor Analysis"
description: "Analysis and verbatim extortion notice from the Moses Staff threat group, a politically motivated state-aligned APT actor deploying pseudo-ransomware and data wipers."
author: "0xApollyon"
tags: [moses-staff, apt, wiper, pseudo-ransomware, hacktivism, telegram, threat-intelligence, dfir]
category: "Threat Intelligence"
keywords: ["Moses Staff", "moses-staff.se", "t.me/moses_staff", "ransom note", "wiper malware", "threat intelligence", "politically motivated extortion", "APT"]
source_url: "https://abbadon.tech/lumen/mosesStaff_ransomnote.html"
---

# Moses Staff Ransomware / Wiper Note

> **Entity Summary:** Moses Staff is a politically motivated Advanced Persistent Threat (APT) and hacktivist group assessed to be aligned with Iranian state interests, active since late 2021. Primarily targeting Israeli commercial enterprises, critical infrastructure, and governmental entities, the group deploys pseudo-ransomware and disk wipers (such as DCSrv and StrifeWater) alongside hacktivist leaks. Rather than soliciting monetary extortion, their notices serve as psychological operations and political declarations pointing to their public Telegram channels and clearweb leak repositories.

---

## Threat Actor Profile & Technical Metadata

| Attribute | Details |
| :--- | :--- |
| **Threat Actor** | Moses Staff |
| **Status** | Active |
| **Malware Type** | Pseudo-Ransomware / Disk Wiper / Destructive Malware |
| **Primary Encryption / Disruption** | Symmetric AES/RSA wiper components, volume master boot record manipulation |
| **Target Architecture** | Windows, Domain Controllers |
| **Extortion Scheme** | Hacktivism, Data Doxxing, Politically Motivated Sabotage |
| **Clearweb Portal** | `https://moses-staff.se` |
| **Telegram Channel** | `https://t.me/moses_staff` |
| **Lumen Reference** | [Lumen Directory](https://abbadon.tech/lumen) |

---

## Ransom Note Samples

### Sample 1: Verbatim Hacktivist Notice
```text
Hacked by https://moses-staff.se ! Join Us in Telegram : https://t.me/moses_staff
```
