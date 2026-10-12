---
title: "RA World Ransomware Note and Threat Actor Analysis"
description: "Comprehensive threat analysis and verbatim ransom note sample for RA World (formerly RA Group), highlighting their HC-128 eStream and ECC Curve25519 encryption, Babuk code lineage, and qTox/Telegram communications."
author: "0xApollyon"
tags: [ra-world, ra-group, babuk-fork, ransomware, hc-128, ecc-curve25519, threat-intelligence, qtox, dfir]
category: "Threat Intelligence"
keywords: ["RA World", "RA Group ransomware", "Connect_202308", "ransom note", "threat intelligence", "HC-128", "ECC Curve25519", "qTox extortion", "Babuk derivative"]
source_url: "https://abbadon.tech/lumen/raworld_ransomnote.html"
---

# RA World Ransomware Note

> **Entity Summary:** RA World (originally surfacing in early 2023 as RA Group) is a double-extortion ransomware syndicate that utilizes modified source code derived from the leaked Babuk ransomware builder. Employing high-speed cryptographic primitives—specifically the HC-128 eSTREAM stream cipher paired with Elliptic Curve Cryptography (Curve25519)—RA World targets healthcare, manufacturing, pharmaceutical, and financial entities. Extortion communications are managed over qTox and Telegram alongside darknet leak repositories.

---

## Threat Actor Profile & Technical Metadata

| Attribute | Details |
| :--- | :--- |
| **Threat Actor** | RA World (formerly RA Group) |
| **Status** | Active |
| **Primary Encryption** | HC-128 (eSTREAM), ECC Curve25519 |
| **Target Architecture** | Windows, Linux / VMware ESXi |
| **Extortion Scheme** | Double Extortion (Database/Report Exfiltration & Stream Cipher Encryption) |
| **qTox ID** | `9A8B9576F0B3846B4CA8B4FAF9F50F633CE731BBC860E76C09ED31FC1A1ACF2A4DFDD79C20F1` |
| **Telegram Handle** | `@Connect_202308` (`hxxps://t.me/Connect_202308`) |
| **Lumen Reference** | [Lumen Directory](https://abbadon.tech/lumen) |

---

## Ransom Note Samples

### Sample 1: Standard Markdown Extortion Notice
```text
# RA World
----
## Notification
Your data are stolen and encrypted when you read this letter.
We have copied all data to our server.
Don't worry, your data will not be compromised if you do what I want.
But if you don't pay, we will release the data, contact your customers and regulators and destroy your system again.


## What we do?
We stole all laboratory reports from your servers.
We stole all important files from your file server.
We stole some important databases from your sql server.
We encrypt all your files.


## What we want?
Contact us, pay for ransom.
If you pay, we will provide you the programs for decryption and we will delete your data.
If not, we will leak your datas and your company will appear in the list below.
If not, we will email to your customers and report to supervisory authority.

 

## How contact us?
We use qTox and Telegram to contact, you can get more information from qTox office website:
hxxps://qtox.github.io


Our qTox ID is:
9A8B9576F0B3846B4CA8B4FAF9F50F633CE731BBC860E76C09ED31FC1A1ACF2A4DFDD79C20F1


Telegram Account:
@Connect_202308
Link:hxxps://t.me/Connect_202308


We have no other contact.
If there is no contact within 3 days, we will make sample files public.
If there is no contact within 7 days, we will stop communicating and release data in batches.
The longer time, the higher ransom.


## RA World Office Site:
[Permanent address] -
[Temporary address] -


## Information release link:
Sample files:
-


## Unpay Victim List
*** You'll be here too if you don't pay! ***


-
Their files can be downloaded from our site:
[Permanent address] -
[Temporary address] -


You can use Tor Browser to open .onion url.
Ger more information from Tor office website:
hxxps://www.torproject.org
```
