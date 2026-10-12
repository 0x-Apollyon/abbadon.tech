---
title: "Abyss Locker Ransomware - Ransom Note Samples & Threat Intelligence"
description: "Ransom note samples and threat intelligence for Abyss and Abyss Locker V2 ransomware, detailing Salsa20 stream cipher encryption, Linux/ESXi targeting, and Tor negotiation portals."
author: "0xApollyon"
tags: [ransomware, abyss, abyss-locker, threat-intelligence, ransom-note, salsa20, tor, the-lumen-register]
category: "Threat Intelligence"
keywords: ["Abyss ransomware", "Abyss Locker", "Abyss ransom note", "Abyss Locker V2", "The Lumen Register", "Salsa20 encryption", "ESXi ransomware", "Tor negotiation"]
source_url: "https://abbadon.tech/lumen/abyss_ransomnote.html"
---

# Abyss Ransom Note

> **Entity Summary:** Abyss (and its successor variant Abyss Locker V2) is an active ransomware operation targeting enterprise corporate networks, including Linux and VMware ESXi environments. The group utilizes Salsa20 stream cipher encryption and exfiltrates proprietary data prior to encryption, coercing victims into Tor-based negotiations under threat of reputation destruction and public data leaks.

## Threat Profile & Metadata

| Attribute | Details |
| :--- | :--- |
| **Threat Actor** | Abyss (Abyss Locker / Abyss Locker V2) |
| **Status** | Active |
| **Known Encryption** | Salsa20 |
| **Primary Communication** | Tor Hidden Service negotiation portals |
| **Onion Leak Site** | `http://3ev4metjirohtdpshsqlkrqcmxq6zu3d7obrdhglpy5jpbr7whmlfgqd.onion` |
| **Victim Negotiation Portals** | `http://jqlcrn2fsfvxlngdq53rqyrwtwfrulup74xyle54bsvo3l2kgpeeijid.onion`, `http://jwqpucwiolhmivnqt7qwroezymksxfjsbj6pmg2lnnglqpoe26cwnryd.onion` |
| **Lumen Reference** | [abyss_ransomnote.html](https://abbadon.tech/lumen/abyss_ransomnote.html) |

---

## Ransom Note Samples

### Ransomnote 1

```text
We are the Abyss. Your company Servers are crypted and your data has been stolen to our servers. Good news for you: 1) We can restore your entire system. 2) We are not interested in publishing your information. 3) Our motivation is purely financial. 4) We are open to negotiations. 5) We are ready to maintain complete confidentiality of this incident. Let's explain the further steps in the situation: You can seek help from authorities - unfortunately, this path will not lead to a constructive resolution of the situation. They will not assist you with decryption, seize your servers for OPsec, and your company's operations will be halted. Subsequently, the date will be disclosed, leading to fines, legal actions, and reputational damage. OR You initiate negotiations with us, and we reach a mutually beneficial and constructive solution for both parties. You pay a specified amount and receive the full decryption, support throughout the decryption process, proofs that all information on our servers has been deleted, and a guarantee that it will never resurface, ensuring no one learns about this incident. To initiate negotiations, please download the Tor Browser using their official website: https://www.torproject.org/ use these credentials to enter the Chat for text negotiation: http://jqlcrn2fsfvxlngdq53rqyrwtwfrulup74xyle54bsvo3l2kgpeeijid.onion/[snip] There will be no bad news for your company after successful negotiations for both sides. But there will be plenty of those bad news if case of failed negotiations, so don’t think about how to avoid it. Just focus on negotiations, payment and decryption to make all of your problems solved by our specialists within 1 day after payment received: servers and data restored, everything will work good as new.
```

### Ransomnote 2

```text
We are the Abyss Locker V2, professionals in all aspects we perform. Your company Servers are locked and Data has been taken to our servers. This is serious. Good news: - 100% of your Server system and Data will be restored by our Decryption Tool; - for now, your data is secured and safely stored on our server; - nobody in the world is aware about the data leak from your company except you and Abyss Locker team. FAQs: Want to go to authorities for protection? - they will do their job properly, but you will not get any win points out of it, only headaches; they will never make decryption for data or servers, they just can’t. Also, they will take all of your IT infrastructure as a part of their procedures… but still they will not help you at all. Think you can handle it without us by decrypting your servers and data using some IT Solution from third-party non-hackers’ “specialists”? - they will only make significant damage to all of your data; every encrypted file will be corrupted forever. Only our Decryption Tool will make decryption 100% guaranteed; Think your partner IT Recovery Company will do files restoration? - no they will not do restoration, only take 3-4 weeks for nothing; besides all of your data is on our servers and we can publish it at any time; as well as send the info about the data breach from your company servers to your key partners and clients, competitors, media and youtubers, etc. Those actions from our side towards your company will have irreversible negative consequences for your business reputation. You don’t care in any case, because you just don’t want to pay hackers? - We will make you business stop forever by using all of our experience to make your partners, clients, employees and whoever cooperates with your company change their minds by having no choice but to stay away from your company. As a result, in midterm you will have to close your business. So lets get straight to the point. What do we offer in exchange on your payment: - decryption and restoration of all your systems and data within 24 hours with 100% guarantee; - never inform anyone about the data breach out from your company; - after data decryption and system restoration, we will delete all of your data from your servers forever; - provide valuable advising on your company IT protection so no one can attack your again. Now, in order to start negotiations, you need to do the following: - download the Tor Browser using their official website: https://www.torproject.org/ - use these credentials to enter the Chat for text negotiation: http://jwqpucwiolhmivnqt7qwroezymksxfjsbj6pmg2lnnglqpoe26cwnryd.onion/[snip] There will be no bad news for your company after successful negotiations for both sides. But there will be plenty of those bad news if case of failed negotiations, so don’t think about how to avoid it. Just focus on negotiations, payment and decryption to make all of your problems solved by our specialists within 1 day after payment received: servers and data restored, everything will work good as new. ************************************************ [snip]
```
