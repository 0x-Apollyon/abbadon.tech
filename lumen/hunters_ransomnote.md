---
title: "Hunters International Ransomware - Ransom Note Samples & Threat Intelligence"
description: "Comprehensive ransom note samples and threat intelligence for the Hunters International RaaS syndicate, documenting Rust-based Hive code lineage, AES encryption, and multi-portal Tor infrastructure."
author: "0xApollyon"
tags: [ransomware, hunters-international, threat-intelligence, ransom-note, aes, rust, hive-codebase, tor, the-lumen-register]
category: "Threat Intelligence"
keywords: ["Hunters International ransomware", "Hunters International ransom note", "Hive ransomware successor", "The Lumen Register", "AES encryption", "huntersinternational net", "hunters55rdxciehoqzwv7vgyv6nt37tbwax2reroyzxhou7my5ejyid onion"]
source_url: "https://abbadon.tech/lumen/hunters_ransomnote.html"
---

# Hunters International Ransom Note

> **Entity Summary:** Hunters International is a highly active Ransomware-as-a-Service (RaaS) syndicate that emerged in late 2023. Analysis reveals significant source code overlap with the seized Hive ransomware operation, rewritten and modernized in Rust. Employing military-grade AES encryption and vast data exfiltration, Hunters International operates multiple high-availability Tor onion portals and a clearnet mirror site.

## Threat Profile & Metadata

| Attribute | Details |
| :--- | :--- |
| **Threat Actor** | Hunters International |
| **Status** | Active |
| **Known Encryption** | AES |
| **Code Lineage** | Derived from Hive v5 (Rust codebase) |
| **Primary Communication** | Tor Hidden Service portals, Clearnet mirror |
| **Onion Leak Portals** | `https://hunters55rdxciehoqzwv7vgyv6nt37tbwax2reroyzxhou7my5ejyid.onion`<br>`https://hunters55atbdusuladzv7vzv6a423bkh6ksl2uftwrxyuarbzlfh7yd.onion` |
| **Victim Contact Portals** | `https://hunters33dootzzwybhxyh6xnmumopeoza6u4hkontdqu7awnhmix7ad.onion`<br>`https://hunters33mmcwww7ek7q5ndahul6nmzmrsumfs6aenicbqon6mxfiqyd.onion` |
| **Clearnet Leak Portal** | [huntersinternational.net](https://huntersinternational.net) |
| **Contact Emails** | `oyewolelawrence@gmail.com`, `cacmountofvictory@gmail.com` |
| **Lumen Reference** | [hunters_ransomnote.html](https://abbadon.tech/lumen/hunters_ransomnote.html) |

---

## Ransom Note Samples

### Ransomnote 1

```text
1. WHAT HAPPENED? <<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<

Your company's network has been compromised by the HUNTERS INTERNATIONAL group.
All files are encrypted using a military-grade AES encryption algorithm.
A large amount of sensitive data was exfiltrated.

We usually download:

- Employees personal data: CVs, DL, SSN, PII, NDA contracts, etc.
- Financial information: documents, payrolls, bank statements, bills, transfers,
  budgets, annual reports, etc.
- Customer data: contracts, PII, contacts, purchase agreements, etc.
- Confidential: source code, trade secrets, technology, blueprints, documents, 
  etc.
- Work files, databases, legal documents, corporate correspondence.
- Accounting data.
- Audit reports.



2. WHAT DO WE OFFER <<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<

To prevent exfiltrated data from being disclosed and to decrypt all the files 
you need to make a payment. Contact us following the instructions:

1) Install and run “Tor Browser” from https://www.torproject.org/download/

2) Go to a dedicated website:
https://hunters33mmcwww7ek7q5ndahul6nmzmrsumfs6aenicbqon6mxfiqyd.onion/
https://hunters33dootzzwybhxyh6xnmumopeoza6u4hkontdqu7awnhmix7ad.onion/ (mirror)

3) Log in using the credentials: [snip]:[snip]



3. WHAT IF NOT? <<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<

We have the most powerful data leak site on the Internet. There are a lot of 
journalholders, researchers and other hackers.

https://hunters55rdxciehoqzwv7vgyv6nt37tbwax2reroyzxhou7my5ejyid.onion/
https://huntersinternational.net/ (mirror)

An incomplete list of risks you are facing in case of non-payment:

 - Loss of customer trust and loyalty.
 - Damage to the company's reputation.
 - Legal consequences and compliance fines.
 - Financial losses and costs associated with data recovery.
 - Impact on competitive advantage and market share.
 - Breach of data privacy regulations and laws.
 - Disruption of business operations.
 - Reduced employee morale and productivity.
 - Potential for intellectual property theft.
 - Loss of trade secrets and proprietary information.



4. KEEP IN MIND <<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<

- Do not try to decrypt using third-party software. You will damage the files.
- Do not report to the Police, FBI, etc. They don't care about your business.
  They simply won't allow you to pay. As a result, you will lose everything.
- Do not hire a recovery company. They can't decrypt without the key.
  They also don't care about your business. They believe that they are
  good negotiators, but it is not. They usually fail. So speak for yourself.
- Do not reject to pay. Exfiltrated files will be disclosed right away.
```

### Ransomnote 2

```text
  _   _ _   _ _   _ _____ _____ ____  ____                                   
 | | | | | | | \ | |_   _| ____|  _ \/ ___|                                  
 | |_| | | | |  \| | | | |  _| | |_) \___ \                                  
 |  _  | |_| | |\  | | | | |___|  _ < ___) |                                 
 |_|_|_|\___/|_|_\_|_|_|_|_____|_|_\_\____/____ ___ ___  _   _    _    _     
 |_ _| \ | |_   _| ____|  _ \| \ | |  / \|_   _|_ _/ _ \| \ | |  / \  | |    
  | ||  \| | | | |  _| | |_) |  \| | / _ \ | |  | | | | |  \| | / _ \ | |    
  | || |\  | | | | |___|  _ <| |\  |/ ___ \| |  | | |_| | |\  |/ ___ \| |___ 
 |___|_| \_| |_| |_____|_| \_\_| \_/_/   \_\_| |___\___/|_| \_/_/   \_\_____|
                                                                             
To contact us follow the instructions:

1) Install and run “Tor Browser” from https://www.torproject.org/download/
2) Go to https://hunters33mmcwww7ek7q5ndahul6nmzmrsumfs6aenicbqon6mxfiqyd.onion/
or https://hunters33dootzzwybhxyh6xnmumopeoza6u4hkontdqu7awnhmix7ad.onion/
3) Log in using the credentials: [snip]

---
Don't waste time. Inform your CEO about the incident ASAP. Show Data Leak Site: 
https://hunters55rdxciehoqzwv7vgyv6nt37tbwax2reroyzxhou7my5ejyid.onion/
or https://hunters55atbdusuladzv7vzv6a423bkh6ksl2uftwrxyuarbzlfh7yd.onion/
```

### Ransomnote 3

```text
  _   _ _   _ _   _ _____ _____ ____  ____                                   
 | | | | | | | \ | |_   _| ____|  _ \/ ___|                                  
 | |_| | | | |  \| | | | |  _| | |_) \___ \                                  
 |  _  | |_| | |\  | | | | |___|  _ < ___) |                                 
 |_|_|_|\___/|_|_\_|_|_|_|_____|_|_\_\____/____ ___ ___  _   _    _    _     
 |_ _| \ | |_   _| ____|  _ \| \ | |  / \|_   _|_ _/ _ \| \ | |  / \  | |    
  | ||  \| | | | |  _| | |_) |  \| | / _ \ | |  | | | | |  \| | / _ \ | |    
  | || |\  | | | | |___|  _ <| |\  |/ ___ \| |  | | |_| | |\  |/ ___ \| |___ 
 |___|_| \_| |_| |_____|_| \_\_| \_/_/   \_\_| |___\___/|_| \_/_/   \_\_____|
                                                                             
To contact us follow the instructions:

1) Install and run “Tor Browser” from https://www.torproject.org/download/
2) Go to https://hunters33mmcwww7ek7q5ndahul6nmzmrsumfs6aenicbqon6mxfiqyd.onion/
3) Log in using the credentials: [snip]

---
Don't waste time. Inform your CEO about the incident ASAP. Show Data Leak Site: 
https://hunters55rdxciehoqzwv7vgyv6nt37tbwax2reroyzxhou7my5ejyid.onion/
```
