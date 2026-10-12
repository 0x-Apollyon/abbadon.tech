---
title: "Ragnar Locker Ransomware Note and Threat Actor Analysis"
description: "Comprehensive threat intelligence and verbatim ransom note samples for Ragnar Locker, detailing Salsa20 encryption, enterprise double extortion, Tox communication, and law enforcement takedown history."
author: "0xApollyon"
tags: [ragnar-locker, ragnar, ransomware, salsa20, rsa-2048, threat-intelligence, tox-chat, law-enforcement-seizure, dfir]
category: "Threat Intelligence"
keywords: ["Ragnar Locker", "Ragnar ransomware", "RAGNAR_LOCKER", "RAGNAR SECRET", "ransom note", "threat intelligence", "Salsa20", "RSA 2048", "Europol seizure"]
source_url: "https://abbadon.tech/lumen/ragnar_ransomnote.html"
---

# Ragnar Locker Ransomware Note

> **Entity Summary:** Ragnar Locker was one of the earliest pioneers of modern double extortion, active between late 2019 and October 2023 before being disrupted in a sweeping multinational operation led by Europol, the FBI, and French gendarmerie. The syndicate targeted critical enterprise environments, energy distributors, and multinational healthcare providers using custom Salsa20 and RSA-2048 cryptography, often executing payloads inside virtualized VirtualBox environments to evade endpoint detection.

---

## Threat Actor Profile & Technical Metadata

| Attribute | Details |
| :--- | :--- |
| **Threat Actor** | Ragnar Locker (`RAGNAR_LOCKER`) |
| **Status** | Disrupted / Seized (International Law Enforcement Operation, Oct 2023) |
| **Primary Encryption** | Salsa20, RSA 2048 |
| **Target Architecture** | Windows, VirtualBox Guest VM Evasion |
| **Extortion Scheme** | Targeted Double Extortion (Multi-Terabyte Exfiltration & Intermittent Salsa20 Encryption) |
| **Communication Channels** | Tox Messenger (`qTOX`), Dedicated Tor Live Chat & News Portals |
| **Key Markers** | `---RAGNAR SECRET---` block |
| **Lumen Reference** | [Lumen Directory](https://abbadon.tech/lumen) |

---

## Ransom Note Samples

### Sample 1: Tox Messenger & Fixed Bitcoin Demand
```text
Hello * !

********************

 If you reading this message, then your network was PENETRATED and all of your files and data has been ENCRYPTED
                             
by RAGNAR_LOCKER !

********************

*********What happens with your system ?************

Your network was penetrated, all your files and backups was locked! So from now there is NO ONE CAN HELP YOU to get your files back, EXCEPT US.
You can google it, there is no CHANCES to decrypt data without our SECRET KEY.

But don't worry ! Your files are NOT DAMAGED or LOST, they are just MODIFIED. You can get it BACK as soon as you PAY.
We are looking only for MONEY, so there is no interest for us to steel or delete your information, it's just a BUSINESS $-)

HOWEVER you can damage your DATA by yourself if you try to DECRYPT by any other software, without OUR SPECIFIC ENCRYPTION KEY !!!

Also, all of your sensitive and private information were gathered and if you decide NOT to pay,
we will upload it for public view !

****

***********How to get back your files ?******

To decrypt all your files and data you have to pay for the encryption KEY :

BTC wallet for payment: *
Amount to pay (in Bitcoin): 25

****

***********How much time you have to pay?**********

* You should get in contact with us within 2 days after you noticed the encryption to get a better price.

* The price would be increased by 100% (double price) after 14 Days if there is no contact made.
 
* The key would be completely erased in 21 day if there is no contact made or no deal made.
Some sensetive information stolen from the file servers would be uploaded in public or to re-seller.

****

***********What if files can't be restored ?******

To prove that we really can decrypt your data, we will decrypt one of your locked files !
Just send it to us and you will get it back FOR FREE.

The price for the decryptor is based on the network size, number of employees, annual revenue.
Please feel free to contact us for amount of BTC that should be paid.

****

! IF you don't know how to get bitcoins, we will give you advise how to exchange the money.


!!!!!!!!!!!!!
! HERE IS THE SIMPLE MANUAL HOW TO GET CONTCAT WITH US !
!!!!!!!!!!!!!

1) Go to the official website of TOX messenger ( hxxps://tox.chat/download.html )

2) Download and install qTOX on your PC, choose the platform ( Windows, OS X, Linux, etc. )

3) Open messenger, click "New Profile" and create profile.

4) Click "Add friends" button and search our contact *

5) For identification, send to our support data from ---RAGNAR SECRET---

IMPORTANT ! IF for some reasons you CAN'T CONTACT us in qTOX, here is our reserve mailbox ( * ) send a message with a data from ---RAGNAR SECRET---

WARNING!

-Do not try to decrypt files with any third-party software (it will be damaged permanently)
-Do not reinstall your OS, this can lead to complete data loss and files cannot be decrypted. NEVER!
-Your SECRET KEY for decryption is on our server, but it will not be stored forever. DO NOT WASTE TIME !


********************

---RAGNAR SECRET---
*
---RAGNAR SECRET---

********************
```

### Sample 2: Live Chat & 10TB Data Leak Notice
```text
*******
HELLO *** !
 If you reading this message, then your network was PENETRATED and all of your files and data has been ENCRYPTED

by RAGNAR_LOCKER !

*******

!!!!! WARNING !!!!!

DO NOT Modify, rename, copy or move any files or you can DAMAGE them and decryption will be impossible.
DO NOT use any third party or public decryption software, it also may damage files.
DO NOT Shutdown or reset your system
-------

There is ONLY ONE possible way to get back your files - contact us and pay for our special decryption key !
For your GUARANTEE we will decrypt 2 of your files FOR FREE, as a proof of our capabilities

Don't waste your TIME, the link for contacting us will be deleted if there is no contact made in closest future and you will never restore your DATA.
HOWEVER if you will contact us within 2 day since get penetrated - you can get a very SPECIAL PRICE.

ATTENTION !
We had downloaded more than 10TB of data from your fileservers and if you don't contact us for payment, we will publish it or sell to interested parties.
Here is just a small part of your files that we have, for a proof (use Tor Browser for open the link) : -

We gathered the most sensitive and confidential information about your transactions, billing, contracts, clients and partners. And be assure that if you wouldn't pay,
all files and documents would be publicated for everyones view and also we would notify all your clients and partners about this leakage with direct links.
So if you want to avoid such a harm for your reputation, better pay the amount that we asking for.

==========
! HERE IS THE SIMPLE MANUAL HOW TO GET CONTACT WITH US VIA LIVE CHAT !
!!!!!

a) Download and install TOR browser from this site : hxxps://torproject.org
b) For contact us via LIVE CHAT open our website : -
c) For visit our NEWS PORTAL with your data, open this website : -
d) If Tor is restricted in your area, use VPN

When you open LIVE CHAT website follow rules :

Follow the instructions on the website.
At the top you will find CHAT tab.
Send your message there and wait for response (we are not online 24/7, So you have to wait for your turn).

*******

---RAGNAR SECRET---
-
---RAGNAR SECRET---

*******
```

### Sample 3: Enterprise Doxxing & News Portal Leak Notice
```text
************************************************
HELLO - !
IF YOU ARE READING THIS, IT'S MEAN YOUR DATA WAS ENCRYPTED AND YOU SENSITIVE PRIVATE INFORMATION WAS STOLEN!
READ CAREFULLY THE WHOLE INSTRUCTION NOTES TO AVOID DIFFICULTIES WITH YOUR DATA

by RAGNAR_LOCKER !

************************************************
*YOU HAVE TO CONTACT US via LIVE CHAT IMMEDIATELY TO RESOLVE THIS CASE AND MAKE A DEAL*
(contact information you will find at the bottom of this notes)

!!!!! WARNING !!!!!

DO NOT Modify, rename, copy or move any files or you can DAMAGE them and decryption will be impossible.
DO NOT Use any third-party or public Decryption software, it also may DAMAGE files.
DO NOT Shutdown or Reset your system, it can DAMAGE files
-------------------------------------

There is ONLY ONE possible way to get back your files - contact us and pay for the special DECRYPTION KEY !
For your GUARANTEE we will decrypt 2 of your files FOR FREE, as a proof that it Works.

Don't waste your TIME, the link for contact us will be deleted if there is no contact made in closest time and you will NEVER restore your DATA.
!!! HOWEVER if you will contact us within 2 day since get penetrated - you can get a very SPECIAL PRICE.

  ! WARNING !
Whole your network was fully COMPROMISED!

 We has DOWNLOADED more than 2 TB of your PRIVATE SENSITIVE Data, including your Billing info, Insuranse cases, Financial reports,
Business audit, Banking Accounts! Also we have corporate correspondence, information about your clients such as AXA Equitable, Abbot Laboratories, AIG, Amazon,
Boston Scientific, Facebook, J & J, SONOCO, Estee Lauder and many others.
We got even more info about your partners and even about your staff, there are some screenshots just as a proofs of what we got on you.
Screenshots:
-

-------------------------------------
Whole data that gathered from your private files and directories could be published in MASS MEDIA for BREAKING NEWS! Yours partners, clients and investors would be notified about LEAK.
However if we make a deal everything would be kept in secret and all your data will be restored.

You can take a look for some more examples of what we have, right now it's a private hidden page, but it could become accessable for Public View if you decide NOT pay.
Use Tor Browser to open the link: -
to view the page's content use password: -

==========================================
! HERE IS THE SIMPLE MANUAL HOW TO GET CONTACT WITH US VIA LIVE CHAT !
!!!!!!!!!!!!!!!!!!!!!!!!

a) Download and install TOR browser from this site : hxxps://torproject.org
b) For contact us via LIVE CHAT open our website : -
c) For visit our NEWS PORTAL with your data, open this website : -  ( password: - )
d) If Tor is restricted in your area, use VPN

When you open LIVE CHAT website follow rules :

Follow the instructions on the website.
At the top you will find CHAT tab.
Send your message there and wait for response (we are not online 24/7, So you have to wait for your turn).
```
