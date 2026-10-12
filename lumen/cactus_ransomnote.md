---
title: "Cactus Ransomware - Ransom Note Samples & Threat Intelligence"
description: "Comprehensive ransom note samples and threat intelligence for the Cactus ransomware operation, documenting self-encrypting binary evasion, AES-256 and RSA-1024 encryption, and Tox/Sonarchat communications."
author: "0xApollyon"
tags: [ransomware, cactus, threat-intelligence, ransom-note, aes-256, rsa-1024, tox, sonarchat, the-lumen-register]
category: "Threat Intelligence"
keywords: ["Cactus ransomware", "Cactus ransom note", "Cactus threat actor", "The Lumen Register", "AES 256", "RSA 1024", "Cactus_Support Sonarchat", "cactus mexicomail"]
source_url: "https://abbadon.tech/lumen/cactus_ransomnote.html"
---

# Cactus Ransom Note

> **Entity Summary:** Cactus is a highly active, evasive ransomware group operating since early 2023. Noted for novel self-encryption techniques where the ransomware binary itself is encrypted with 7-Zip and decrypted in-memory using an execution flag to bypass antivirus engines, Cactus leverages AES-256 and RSA-1024 to lock victim data. The group relies on Tox, Sonarchat, protonmail, and Tor leak portals for double extortion.

## Threat Profile & Metadata

| Attribute | Details |
| :--- | :--- |
| **Threat Actor** | Cactus |
| **Status** | Active |
| **Known Encryption** | AES 256, RSA 1024 |
| **Evasion Tactics** | In-memory payload decryption, VPN vulnerability exploitation |
| **Primary Communication** | Tox Messenger, Sonarchat, Email, Tor leak blog |
| **Onion Leak Portals** | `http://cactusbloguuodvqjmnzlwetjlpj6aggc6iocwhuupb47laukux7ckid.onion`<br>`http://cactus5dqnqkppa5ayckiyk6dttpqwczdqphv5mxh4dkk5ct544q5aad.onion/` |
| **Sonarchat Portal** | `http://sonarmsng5vzwqezlvtu2iiwwdn3dxkhotftikhowpfjuzg7p3ca5eid.onion/contact/Cactus_Support` |
| **Tox ID** | `7367B422CD7498D5F2AAF33F58F67A332F8520CF0279A5FBB4611E0121AE421AE1D49ACEABB2` |
| **Contact Emails** | `cactus787835@proton.me`, `halielang@protonmail.com`, `cactus@mexicomail.com` |
| **Lumen Reference** | [cactus_ransomnote.html](https://abbadon.tech/lumen/cactus_ransomnote.html) |

---

## Ransom Note Samples

### Ransomnote 1

```text
Your systems were accessed and encrypted by Cactus.
Do not interrupt the encryption process, don't stop or reboot your machines.
Otherwise the data may be corrupted and unrecoverable.
The best you can do is wait until encryption is finished to keep your files safe.
Besides, we have downloaded a huge pack of confidential information from your systems.
To recover your files and prevent disclosure of your sensitive data contact us via email: halielang@protonmail.com
Your unique ID: 
Backup contacts: EMAIL: cactus787835@proton.me
TOX (https://tox.chat/):
7367B422CD7498D5F2AAF33F58F67A332F8520CF0279A5FBB4611E0121AE421AE1D49ACEABB2
```

### Ransomnote 2

```text
Your systems were accessed and encrypted by Cactus.
Do not interrupt the encryption process, don't stop or reboot your machines.
Otherwise the data may be corrupted and unrecoverable.
The best you can do is wait until encryption is finished to keep your files safe.
Besides, we have downloaded a huge pack of confidential information from your systems.
To recover your files and prevent disclosure of your sensitive data contact us via email: cactus@mexicomail.com
Your unique ID: 
Backup contacts: EMAIL: cactus787835@proton.me
TOX (https://tox.chat/):
7367B422CD7498D5F2AAF33F58F67A332F8520CF0279A5FBB4611E0121AE421AE1D49ACEABB2
```

### Ransomnote 3

```text
Your systems were accessed and encrypted by Cactus.
To recover your files and prevent data disclosure contact us via email: cactus@mexicomail.com
Your unique ID reference: 
Backup contact: TOX (https://tox.chat/):
7367B422CD7498D5F2AAF33F58F67A332F8520CF0279A5FBB4611E0121AE421AE1D49ACEABB2
```

### Ransomnote 4

```text
Your systems were accessed and encrypted by Cactus.
Do not interrupt the encryption process, don't stop or reboot your machines.
Otherwise the data may be corrupted and unrecoverable.
The best you can do is wait until encryption is finished to keep your files safe.
Besides, we have downloaded a huge pack of confidential information from your systems.
To recover your files and prevent disclosure of your sensitive data contact us via email: cactus@mexicomail.com 
Your unique ID: 
Backup contacts: http://sonarmsng5vzwqezlvtu2iiwwdn3dxkhotftikhowpfjuzg7p3ca5eid.onion/contact/Cactus_Support 
TOX (https://tox.chat/): 7367B422CD7498D5F2AAF33F58F67A332F8520CF0279A5FBB4611E0121AE421AE1D49ACEABB2
```

### Ransomnote 5

```text
Your systems were accessed and encrypted by Cactus.
Do not interrupt the encryption process, don't stop or reboot your machines.
Otherwise the data may be corrupted and unrecoverable.
The best you can do is wait until encryption is finished to keep your files safe
.
Besides, we have downloaded a huge pack of confidential information from your sy
stems.
Your data will be sold or published in our blog https:\cactusbloguuodvqjmnzlwetjlpj6aggc6iocwhuupb47laukux7ckid.onion in case of non-payment
To recover your files and prevent disclosure of your sensitive data contact us via email: cactus@mexicomail.com
Your unique ID: [snip]
Backup contacts: http://sonarmsng5vzwqezlvtu2iiwwdn3dxkhotftikhowpfjuzg7p3ca5eid.onion/contact/Cactus_Support
TOX (https://tox.chat/):
7367B422CD7498D5F2AAF33F58F67A332F8520CF0279A5FBB4611E0121AE421AE1D49ACEABB2
```
