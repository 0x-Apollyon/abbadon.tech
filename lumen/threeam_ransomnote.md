---
title: "3AM (ThreeAM) Ransomware Note and Threat Actor Analysis"
description: "Comprehensive threat profile and verbatim ransom note sample for 3AM (ThreeAM) ransomware, featuring occult ASCII graphics, ChaCha20/RSA encryption, LockBit affiliate origins, and Tor recovery infrastructure."
author: "0xApollyon"
tags: [threeam, 3am, ransomware, chacha20, rsa, threat-intelligence, tor-negotiation, dfir]
category: "Threat Intelligence"
keywords: ["ThreeAM", "3AM ransomware", "threeam7fj33rv5twe5ll7gcrp3kkyyt6ez5stssixnuwh4v3csxdwqd.onion", "ThreeAM@onionmail.org", "ransom note", "threat intelligence", "ChaCha20", "RSA", "cyber extortion"]
source_url: "https://abbadon.tech/lumen/threeam_ransomnote.html"
---

# 3AM (ThreeAM) Ransomware Note

> **Entity Summary:** 3AM (also known as ThreeAM) is an extortionate ransomware family discovered in late 2023 by Symantec threat researchers after an affiliate attempted and failed to deploy LockBit Black before falling back to 3AM. Written in 64-bit C++, the payload uses hybrid 256-bit ChaCha20 and RSA cryptography. Extortion notices are distinguished by occult-themed ASCII clock and entity graphics, declaring "3 am - The time of mysticism," and directing victims to a dedicated Tor recovery gateway.

---

## Threat Actor Profile & Technical Metadata

| Attribute | Details |
| :--- | :--- |
| **Threat Actor** | 3AM (ThreeAM) |
| **Status** | Active |
| **Primary Encryption** | ChaCha20, RSA |
| **Target Architecture** | Windows |
| **Extortion Scheme** | Double Extortion (Confidential Local Data Exfiltration & File Locking) |
| **Negotiation Portal (Tor)**| `http://threeam7fj33rv5twe5ll7gcrp3kkyyt6ez5stssixnuwh4v3csxdwqd.onion/recovery` |
| **Communication Email** | `ThreeAM@onionmail.org` |
| **Lumen Reference** | [Lumen Directory](https://abbadon.tech/lumen) |

---

## Ransom Note Samples

### Sample 1: Standard 3AM Notice with ASCII Art
```text
                                   .,,,.    
                              .,,,**,,,,,*,*    
                           **,****,,.*,,,,,,,,,,   
                        **,,,,,***,..,***,,,,,,,,,, 
                      ..,*,,,,,***, ,,**,,,,,,,,,,,,.   
                      ,,,****,*,,.. ......,,*,,,,,,,,,  
                     *,,,,***,,,,        .,*,,,,,,,,,,, 
                  .,,,,,,.                     ,,, .,,,,   
                .*,,*.                           .,,  .,   
               ,*,                                 .,,     
              ,,,        *.    .*,     **.   .(      .,,   
              ,,,          #..#.        ..#,/,         ,,  
              ,,           .#(,          .%,,#.        ,,. 
             ,,.          %    *,..   ..%      #        *, 
              ,,                                         ,, 
              ,, .         (,      .   ..    .%,      .  ,, 
              .,  . ,       *(*,/  . *   .(**(,       ,  ,  
               ,  . ,        #/. (,*(,,..*#.        , .,   
                ..  .,,          ,/(#/*            . ,  .   
             .,.  .   ..            /              ,.   .,, 
         *,,**,,**   .   .,                      ,.*  .,,,,,,. 
     ,,,,,,***,,,**,,  ,   ..                  , .  ,,,,,,,,,,,,, 
   ,**,,,,****,,,,,**,,,      .             .     ,,,,,,  ,,,,,,,,,,,.   
   ,,,,*,,,,*,*,**,,,,****,**,.                 *,,,.    ,,,,,,.,,,,.,,,.   
.  ,,,, ,,,,,,***,,,,,*.*,,                   ,.        .,,       ,,,.,,,   
,  ,,,. ,*,,*,,,,,,,,,,,,.*                 .          .        ,,.    .,,  
, .,,. .,*,     .,.,*   ,,,                                             ,.  
.,,,,.            ,, ,.                                               .     
,,,.   ..             ,                                                        
                      ,                                            .,        

Hello. "3 am" The time of mysticism, isn't it?

All your files are mysteriously encrypted, and the systems "show no signs of life", the backups disappeared. But we can correct this very quickly and return all your files and operation of the systems to original state.

All your attempts to restore data by himself will definitely lead to their damage and the impossibility of recovery. We are not recommended to you to do it on our own!!! (or do at your own peril and risk).


There is another important point: we stole a fairly large amount of sensitive data from your local network: financial documents; personal information of your employees, customers, partners; work documentation, postal correspondence and much more.

We prefer to keep it secret, we have no goal to destroy your business. Therefore can be no leakage on our part.

We propose to reach an agreement and conclude a deal.


Otherwise, your data will be sold to darknet. One can only guess how they will be used.

Please contact us as soon as possible, using Tor-browser:
http://threeam7fj33rv5twe5ll7gcrp3kkyyt6ez5stssixnuwh4v3csxdwqd.onion/recovery

Access key:
[snip]
```
