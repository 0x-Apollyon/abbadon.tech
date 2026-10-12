---
title: "DragonForce Ransomware - Ransom Note Sample & Threat Intelligence"
description: "Ransom note sample and threat intelligence for the DragonForce ransomware group, documenting double extortion practices, database targeting, Tox support, and Tor client negotiation portals."
author: "0xApollyon"
tags: [ransomware, dragonforce, threat-intelligence, ransom-note, tox, tor, double-extortion, the-lumen-register]
category: "Threat Intelligence"
keywords: ["DragonForce ransomware", "DragonForce ransom note", "DragonForce threat actor", "The Lumen Register", "Tox support", "3pktcrcbmssvrnwe5skburdwe2h3v6ibdnn5kbjqihsg6eu6s6b7ryqd onion", "z3wqggtxft7id3ibr7srivv5gjof5fwg76slewnzwwakjuf3nlhukdid onion"]
source_url: "https://abbadon.tech/lumen/dragonforce_ransomnote.html"
---

# DragonForce Ransom Note

> **Entity Summary:** DragonForce is an active cyber extortion group that emerged in late 2023. Not to be confused with the pro-Palestinian hacktivist collective of the same name, this ransomware operation leverages modified LockBit 3.0 code to compromise critical corporate databases (Oracle, MSSQL), demanding Bitcoin ransoms via Tor-based client portals and dedicated Tox support channels.

## Threat Profile & Metadata

| Attribute | Details |
| :--- | :--- |
| **Threat Actor** | DragonForce |
| **Status** | Active |
| **Known Encryption** | Strong asymmetric/symmetric cipher suite |
| **Primary Communication** | Tor Hidden Service client area, Tox messenger |
| **Onion Leak Blog** | `http://z3wqggtxft7id3ibr7srivv5gjof5fwg76slewnzwwakjuf3nlhukdid.onion` |
| **Victim Contact Portal** | `http://3pktcrcbmssvrnwe5skburdwe2h3v6ibdnn5kbjqihsg6eu6s6b7ryqd.onion` |
| **Support Tox ID** | `1C054B722BCBF41A918EF3C485712742088F5C3E81B2FDD91ADEA6BA55F4A856D90A65E99D20` |
| **Lumen Reference** | [dragonforce_ransomnote.html](https://abbadon.tech/lumen/dragonforce_ransomnote.html) |

---

## Ransom Note Samples

### Ransom Note

```text
Hello! 

Your files (orcl, IADeAPP, [snip] dbs) have been stolen from your network and encrypted with a strong algorithm. We work for money and are not associated with politics.
All you need to do is contact us and pay.

--- Our communication process:

	1. You contact us.
	2. We send you a list of files that were stolen.
	3. We decrypt 1 file to confirm that our decryptor works.
	4. We agree on the amount, which must be paid using BTC.
	5. We delete your files, we give you a decryptor.
	6. We give you a detailed report on how we compromised your company, and recommendations on how to avoid such situations in the future.
   
--- Client area (use this site to contact us):

	Link for Tor Browser: http://3pktcrcbmssvrnwe5skburdwe2h3v6ibdnn5kbjqihsg6eu6s6b7ryqd.onion
	>>> Use this ID: [snip] to begin the recovery process.
	
	* In order to access the site, you will need Tor Browser, 
	  you can download it from this link: https://www.torproject.org/

--- Additional contacts:

	Support Tox: 1C054B722BCBF41A918EF3C485712742088F5C3E81B2FDD91ADEA6BA55F4A856D90A65E99D20

--- Recommendations: 

	DO NOT RESET OR SHUTDOWN - files may be damaged.
	DO NOT RENAME OR MOVE the encrypted and readme files.
	DO NOT DELETE readme files.

--- Important:

	If you refuse to pay or do not get in touch with us, we start publishing your files.
	21/01/2024 00:00 UTC the decryptor will be destroyed and the files will be published on our blog.
	
	Blog: http://z3wqggtxft7id3ibr7srivv5gjof5fwg76slewnzwwakjuf3nlhukdid.onion

Sincerely, 01000100 01110010 01100001 01100111 01101111 01101110 01000110 01101111 01110010 01100011 01100101
```
