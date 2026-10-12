---
title: "Lynx Ransomware Note and Threat Actor Analysis"
description: "Comprehensive threat profile and verbatim ransom note samples from the Lynx ransomware operation, including darknet negotiation portals, multi-mirror leak sites, and extortion channels."
author: "0xApollyon"
tags: [lynx, ransomware, double-extortion, data-leak, threat-intelligence, tor-negotiation, dfir]
category: "Threat Intelligence"
keywords: ["Lynx", "Lynx ransomware", "lynxblog.net", "ransom note", "threat intelligence", "cyber extortion", "data leak portal"]
source_url: "https://abbadon.tech/lumen/lynx_ransomnote.html"
---

# Lynx Ransomware Note

> **Entity Summary:** Lynx is a double-extortion ransomware actor that surfaced in mid-2024. The threat group encrypts corporate endpoints while exfiltrating proprietary documents. Known for maintaining highly redundant, distributed communication infrastructure, Lynx operates multiple fallback Tor negotiation gateways and mirror sites alongside clearweb disclosures (`lynxblog.net`) and ProtonMail backup communications.

---

## Threat Actor Profile & Technical Metadata

| Attribute | Details |
| :--- | :--- |
| **Threat Actor** | Lynx |
| **Status** | Active |
| **Primary Encryption** | Proprietary / Not Publicly Specified |
| **Target Architecture** | Windows, Linux |
| **Extortion Scheme** | Double Extortion (Confidential Data Exfiltration & File Encryption) |
| **Leak Site (Clearweb)**| `http://lynxblog.net/` |
| **Leak Site (Tor)** | `http://lynxbllrfr5262yvbgtqoyq76s7mpztcqkv6tjjxgpilpma7nyoeohyd.onion/disclosures`<br>`http://lynxblogxstgzsarfyk2pvhdv45igghb4zmthnzmsipzeoduruz3xwqd.onion/` |
| **Negotiation Portal (Tor)**| `http://lynxch2k5xi35j7hlbmwl7d6u2oz4vp2wqp6qkwol624cod3d6iqiyqd.onion/login`<br>`http://lynxchatly4zludmhmi75jrwhycnoqvkxb4prohxmyzf4euf5gjxroad.onion/login` |
| **Email Backup** | `martina.lestariid1898@proton.me` |
| **Lumen Reference** | [Lumen Directory](https://abbadon.tech/lumen) |

---

## Ransom Note Samples

### Sample 1: Standard Notice with ProtonMail Backup
```text
Your data is stolen and encrypted.
Your unique identificator is [snip]
Use this TOR site to contact with us:
http://lynxch2k5xi35j7hlbmwl7d6u2oz4vp2wqp6qkwol624cod3d6iqiyqd.onion/login

Use this email to contact with us:
martina.lestariid1898@proton.me

Our blog
 ~ TOR Network: http://lynxbllrfr5262yvbgtqoyq76s7mpztcqkv6tjjxgpilpma7nyoeohyd.onion/disclosures
 ~ Mirror #1: http://lynxblog.net/
```

### Sample 2: Multi-Mirror Infrastructure Notice
```text
Your data is stolen and encrypted.
Download TOR Browser to contact with us.

ID
 ~ [snip]

Chat site:
 ~ TOR Network: http://lynxchatly4zludmhmi75jrwhycnoqvkxb4prohxmyzf4euf5gjxroad.onion/login
 ~ TOR Mirror #1: http://lynxchatfw4rgsclp4567i4llkqjr2kltaumwwobxdik3qa2oorrknad.onion/login
 ~ TOR Mirror #2: http://lynxchatohmppv6au67lloc2vs6chy7nya7dsu2hhs55mcjxp2joglad.onion/login
 ~ TOR Mirror #3: http://lynxchatbykq2vycvyrtjqb3yuj4ze2wvdubzr2u6b632trwvdbsgmyd.onion/login
 ~ TOR Mirror #4: http://lynxchatde4spv5x6xlwxf47jdo7wtwwgikdoeroxamphu3e7xx5doqd.onion/login
 ~ TOR Mirror #5: http://lynxchatdy3tgcuijsqofhssopcepirjfq2f4pvb5qd4un4dhqyxswqd.onion/login
 ~ TOR Mirror #6: http://lynxchatdykpoelffqlvcbtry6o7gxk3rs2aiagh7ddz5yfttd6quxqd.onion/login
 ~ TOR Mirror #7: http://lynxch2k5xi35j7hlbmwl7d6u2oz4vp2wqp6qkwol624cod3d6iqiyqd.onion/login

Our blog:
 ~ TOR Network: http://lynxblogxstgzsarfyk2pvhdv45igghb4zmthnzmsipzeoduruz3xwqd.onion/
 ~ TOR Mirror #1: http://lynxblogco7r37jt7p5wrmfxzqze7ghxw6rihzkqc455qluacwotciyd.onion/
 ~ TOR Mirror #2: http://lynxblogijy4jfoblgix2klxmkbgee4leoeuge7qt4fpfkj4zbi2sjyd.onion/
 ~ TOR Mirror #3: http://lynxblogmx3rbiwg3rpj4nds25hjsnrwkpxt5gaznetfikz4gz2csyad.onion/
 ~ TOR Mirror #4: http://lynxblogoxllth4b46cfwlop5pfj4s7dyv37yuy7qn2ftan6gd72hsad.onion/
 ~ TOR Mirror #5: http://lynxblogtwatfsrwj3oatpejwxk5bngqcd5f7s26iskagfu7ouaomjad.onion/
 ~ TOR Mirror #6: http://lynxblogxutufossaeawlij3j3uikaloll5ko6grzhkwdclrjngrfoid.onion/
 ~ Mirror #7: http://lynxblog.net/
 
```
