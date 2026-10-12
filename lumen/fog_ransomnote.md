---
title: "Fog Ransomware - Ransom Note Sample & Threat Intelligence"
description: "Ransom note sample and threat analysis for Fog ransomware, documenting HC-256 stream cipher and RSA encryption, education/recreation sector targeting, and Tor victim contact portals."
author: "0xApollyon"
tags: [ransomware, fog, threat-intelligence, ransom-note, hc-256, rsa, tor, the-lumen-register]
category: "Threat Intelligence"
keywords: ["Fog ransomware", "Fog ransom note", "Fog threat actor", "The Lumen Register", "HC-256 encryption", "RSA encryption", "xql562evsy7njcsngacphc2erzjfecwotdkobn3m4uxu2gtqh26newid onion"]
source_url: "https://abbadon.tech/lumen/fog_ransomnote.html"
---

# Fog Ransom Note

> **Entity Summary:** Fog is an active ransomware group that surfaced in early 2024, heavily targeting educational institutions, recreation, and commercial businesses. Fog gains initial network access primarily through compromised VPN credentials, using HC-256 stream cipher and RSA encryption to rapidly lock Windows endpoints while managing victim communications through dedicated Tor portals.

## Threat Profile & Metadata

| Attribute | Details |
| :--- | :--- |
| **Threat Actor** | Fog |
| **Status** | Active |
| **Known Encryption** | HC-256, RSA |
| **Initial Access Vector** | Compromised VPN gateways (SonicWall, etc.) |
| **Primary Communication** | Tor Hidden Service negotiation portal |
| **Onion Leak Site** | `http://xbkv2qey6u3gd3qxcojynrt4h5sgrhkar6whuo74wo63hijnn677jnyd.onion` |
| **Victim Contact Portal** | `http://xql562evsy7njcsngacphc2erzjfecwotdkobn3m4uxu2gtqh26newid.onion` |
| **Lumen Reference** | [fog_ransomnote.html](https://abbadon.tech/lumen/fog_ransomnote.html) |

---

## Ransom Note Samples

### Ransom Note

```text
If you are reading this, then you have been the victim of a cyber attack. We call ourselves Fog and we take responsibility for this incident. We are the ones who encrypted your data and also copied some of it to our internal resource. The sooner you contact us, the sooner we can resolve this incident and get you back to work. To contact us you need to have Tor browser installed: 1. Follow this link: xql562evsy7njcsngacphc2erzjfecwotdkobn3m4uxu2gtqh26newid.onion 2. Enter the code: [snip] 3. Now we can communicate safely. If you are decision-maker, you will get all the details when you get in touch. We are waiting for you.
```
