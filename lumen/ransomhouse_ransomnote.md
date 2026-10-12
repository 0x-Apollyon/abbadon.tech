---
title: "RansomHouse Ransomware Note and Threat Actor Analysis"
description: "Comprehensive threat profile and verbatim ransom note samples for RansomHouse (featuring Mario ESXi and White Rabbit strains), detailing extortion tactics, ASCII art, and Tor communication portals."
author: "0xApollyon"
tags: [ransomhouse, mario-esxi, white-rabbit, ransomware, data-extortion, rsa-2048, aes, threat-intelligence, dfir]
category: "Threat Intelligence"
keywords: ["RansomHouse", "Mario ESXi", "White Rabbit ransomware", "ransom note", "threat intelligence", "t.me/ransom_house", "AES", "RSA 2048", "double extortion"]
source_url: "https://abbadon.tech/lumen/ransomhouse_ransomnote.html"
---

# RansomHouse Ransomware Note

> **Entity Summary:** RansomHouse is an extortion syndicate that emerged in December 2021. Presenting itself initially as a "professional mediation" and data-trading marketplace, the group subsequently collaborated with and deployed custom ransomware payloads, including the VMware ESXi-focused "Mario ESXi" locker and the "White Rabbit" ransomware strain. Characterized by elaborate ASCII art in their extortion notes, RansomHouse conducts double-extortion attacks backed by public shaming on Telegram and dedicated Tor repositories.

---

## Threat Actor Profile & Technical Metadata

| Attribute | Details |
| :--- | :--- |
| **Threat Actor** | RansomHouse (Mario ESXi / White Rabbit) |
| **Status** | Active |
| **Primary Encryption** | AES, RSA 2048 |
| **Target Architecture** | Windows, Linux / VMware ESXi |
| **Extortion Scheme** | Double Extortion (Confidential Data Theft & System Encryption), Telegram Public Shaming |
| **Leak Site (Tor)** | `http://xw7au5pnwtl6lozbsudkmyd32n6gnqdngitjdppybudan3x3pjgpmpid.onion/`<br>`http://zohlm7ahjwegcedoz7lrdrti7bvpofymcayotp744qhx6gjmxbuo2yid.onion/` |
| **Negotiation Portal (Tor)**| `http://secxrosqawaefsio3biv2dmi2c5yunf3t7ilwf54czq3v4bi7w6mbfad.onion/`<br>`http://p2tn23lt5zpzzyo4bmnpwgbmxhnifggk5ioizmmaeuz4n2bcyv2q44yd.onion/` |
| **Telegram Channel** | `https://t.me/ransom_house` |
| **Lumen Reference** | [Lumen Directory](https://abbadon.tech/lumen) |

---

## Ransom Note Samples

### Sample 1: Mario ESXi Variant with ASCII Art
```text
--------------------------------------------------------
                     Welcome to the RansomHouse            
                         You are locked by              
                          M A R I O ESXI           
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣠⣴⡾⣻⣿⣿⣿⣿⣯⣍⠛⠻⢷⣦⣀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣴⣿⠟⢁⣾⠟⠋⣁⣀⣤⡉⠻⣷⡀⠀⠙⢿⣷⣄⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⢀⡀⠀⠀⠀⠀⠀⠀⣰⣿⠏⠀⠀⢸⣿⠀⠼⢋⣉⣈⡳⢀⣿⠃⠀⠀⠀⠙⣿⣦⡀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⢰⡿⠿⣷⡀⠀⠀⠀⣼⣿⠃⠀⠀⣀⣤⡿⠟⠛⠋⠉⠉⠙⢛⣻⠶⣦⣄⡀⠀⠘⣿⣷⡀⠀⠀⠀
⢠⣾⠟⠳⣦⣄⢸⡇⠀⠈⣷⡀⠀⣼⣿⡏⢀⣤⡾⢋⣵⠿⠻⢿⠋⠉⠉⢻⠟⠛⠻⣦⣝⠻⣷⣄⠸⣿⣿⠀⠀⠀
⠘⧧⠀⠀⠀⠙⢿⣿⠀⠀⢸⣷⠀⣿⣿⣧⣾⣏⡴⠛⢡⠖⢛⣲⣅⠀⠀⣴⣋⡉⠳⡄⠈⠳⢬⣿⣿⣿⡿⠀⠀⠀
⠀⠘⠷⣤⣀⣀⣀⣽⡶⠛⠛⠛⢷⣿⣿⣿⣿⣏⠀⠀⡏⢰⡿⢿⣿⠀⠀⣿⠻⣿⠀⡷⠀⣠⣾⣿⡿⠛⠷⣦⠀⠀
⠀⠀⢀⣾⠟⠉⠙⣿⣤⣄⠀⢀⣾⠉⠀⢹⣿⣿⣷⠀⠹⡘⣷⠾⠛⠋⠉⠛⠻⢿⡴⢃⣄⣻⣿⣿⣷⠀⠀⢹⡇⠀
⠀⠀⢸⡇⠈⠉⠛⢦⣿⡏⠀⢸⣧⠀⠈⠻⣿⡿⢣⣾⣦⣽⠃⠀⠀⠀⠀⠀⠀⠀⣷⣾⣿⡇⠉⢿⡇⠀⢀⣼⠇⠀
⠀⠀⠘⣷⡠⣄⣀⣼⠇⠀⠀⠀⠻⣷⣤⣀⣸⡇⠀⠹⣿⣿⣦⣀⠀⠀⠀⠀⢀⣴⣿⣿⡟⠀⠀⢸⣷⣾⡿⠃⠀⠀
⠀⠀⠀⠈⠻⢦⣍⣀⣀⣀⡄⠀⣰⣿⡿⠿⢿⣇⠀⠀⠉⠛⠻⣿⣿⡷⠾⣿⣿⡿⠉⠁⠀⠀⢀⣾⠋⠁⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠈⠉⠉⠙⠿⢿⣿⣇⠀⠀⠈⢿⣧⣄⠀⠀⠀⢹⣷⣶⣶⣾⣿⡇⠀⠀⣀⣴⡿⣧⣄⡀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠙⢿⣷⡀⠀⠀⠙⢿⣿⣶⣤⡀⠻⢤⣀⡤⠞⢀⣴⣿⣿⠟⢷⡀⠙⠻⣦⣄⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⢻⣦⠀⢠⡟⠁⠙⢻⣿⠷⠶⣶⠶⠾⠛⠙⣿⠇⠀⠀⢻⡄⠀⠀⠙⢷⡀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣸⣿⡀⣿⠁⣤⣤⡄⢻⡶⠶⠛⠛⠛⠛⠛⣿⢠⣾⣷⣆⢻⡀⠀⠀⠈⣷
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣿⣿⣿⣿⢸⣿⣿⣿⡈⢿⡀⠀⠀⠀⠀⠀⡿⢸⣿⣿⣿⢸⡇⠀⠀⠀⡟
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠉⠉⠉⠈⠉⠉⠉⠁⠈⠁⠀⠀⠀⠀⠈⠁⠈⠉⠉⠉⠀⠁⠀⠀⠈⠁                      
                           Dear [snip],
If you are reading this message, it means that: 
      - your network infrastructure has been compromised, 
      - critical data was leaked, 
      - files are encrypted
--------------------------------------------------------
   The best and only thing you can do is to contact us 
              to settle the matter before any losses occurs.
                                             
Onion Site:
http://xw7au5pnwtl6lozbsudkmyd32n6gnqdngitjdppybudan3x3pjgpmpid.onion/
Telegram Channel:
https://t.me/ransom_house
--------------------------------------------------------
                                  1. THE FOLLOWING IS STRICTLY FORBIDDEN

1.1 EDITING FILES ON HDD. 	
                            Renaming, copying or moving any files 
                            could DAMAGE the cipher and 
                            decryption will be impossible. 
1.2 USING THIRD-PARTY SOFTWARE. 
                            Trying to recover with any software 
                            can also break the cipher and 
                            file recovery will become a problem.
1.3 SHUTDOWN OR RESTART THE PC. 
                            Boot and recovery errors can also damage the cipher. 
                            Sorry about that, but doing so is entirely at your own risk.
--------------------------------------------------------
                                  2. EXPLANATION OF THE SITUATION
2.1 HOW DID THIS HAPPEN
The security of your IT perimeter has been compromised (it's not perfect at all). 
We encrypted your workstations and servers to make the fact of the intrusion visible and to prevent you from hiding critical data leaks.
We spent a lot of time researching and finding out the most important directories of your business, your weak points. 
We have already downloaded a huge amount of critical data and analyzed it. Now its fate is up to you, it will either be deleted or sold, or shared with the media.
2.2 VALUABLE DATA WE USUALLY STEAL:
                            - Databases, legal documents, personal information.
                            - Audit reports.
                            - Any financial documents (Statements, invoices, accounting, transfers etc.).
                            - Work files and corporate correspondence.
                            - Any backups.
			    - Confidential documents.
2.3 TO DO LIST (best practies)
                            - Contact us as soon as possible.
                            - Contact us only in our live chat, otherwise you can run into scammers.
                            - Purchase our decryption tool and decrypt your files. There is no other way to do this.
                            - Realize that dealing with us is the shortest way to success and secrecy.
                            - Give up the idea of using decryption help programs, otherwise you will destroy the system permanently.
                            - Avoid any third-party negotiators and recovery groups. They can become the source of leaks.
--------------------------------------------------------
                                  3. POSSIBLE DECISIONS
3.1 NOT MAKING THE DEAL
                            - After 6 days starting tomorrow your leaked data will be Disclosed or sold.
                            - We will also send the data to all interested supervisory organizations and the media.
                            - Decryption key will be deleted permanently and recovery will be impossible.
                            - Losses from the situation can be measured based on your annual budget.
3.2 MAKING THE WIN-WIN DEAL
                            - You will get the only working Decryption Tool and the how-to-use Manual. 
                            - You will get our guarantees (with log provided) of non-recovarable deletion of all your leaked data.
                            - You will get our guarantees of secrecy and removal of all traces related to the deal in the Internet. 
                            - You will get our security report on how to fix your security breaches.
--------------------------------------------------------
                                  4. EVIDENCE OF THE LEAKAGE
                			In our live chat
http://secxrosqawaefsio3biv2dmi2c5yunf3t7ilwf54czq3v4bi7w6mbfad.onion/?Url=[snip]
--------------------------------------------------------
                                  5. HOW TO CONTACT US
5.1 Download and install TOR Browser https://torproject.org
5.2 Go to our live-chat website at http://secxrosqawaefsio3biv2dmi2c5yunf3t7ilwf54czq3v4bi7w6mbfad.onion/?Url=[snip]
5.3 You can request ftp server access in our live chat to review leaked data samples. 
5.4 In case TOR Browser is restricted in your area use VPN services.
5.5 All leaked Data samples will be Disclosed in 4 Days if you remain silent.
5.6 Your Decryption keys will be permanently destroyed at the moment the leaked Data is Disclosed.
--------------------------------------------------------
                                  6. RESPONSIBILITY
6.1 Breaking critical points of this offer will cause:
                            - Deletion of your decryption keys.
                            - Immediate sale or complete Disclosure of your leaked data.
                            - Notification of government supervision agencies, your competitors and clients.
--------------------------------------------------------                            
```

### Sample 2: White Rabbit Variant with ASCII Rabbit
```text
--------------------------------------------------------------------------
                        Welcome to the RansomHouse            
                            You are locked by              
                         W H I T E  R A B B I T              
                  Knock, Knock. Follow the White Rabbit... 
                                                             
                               (\(\   Come, come now. Crying won't help.                     
                               (-.-)                                 
                               (")(") 

       Dear The [snip] Management,

If you are reading this message, it means that: 
      - your network infrastructure has been compromised, 
      - critical data was leaked, 
      - files are encrypted
--------------------------------------------------------------------------
            The best and only thing you can do is to contact us 
              to settle the matter before any losses occurs.
                                             
Onion Site:
http://zohlm7ahjwegcedoz7lrdrti7bvpofymcayotp744qhx6gjmxbuo2yid.onion/
Telegram Channel:
https://t.me/ransom_house
--------------------------------------------------------------------------

                                  1. THE FOLLOWING IS STRICTLY FORBIDDEN


1.1 EDITING FILES ON HDD. 	
                            Renaming, copying or moving any files 
                            could DAMAGE the cipher and 
                            decryption will be impossible. 

1.2 USING THIRD-PARTY SOFTWARE. 
                            Trying to recover with any software 
                            can also break the cipher and 
                            file recovery will become a problem.

1.3 SHUTDOWN OR RESTART THE PC. 
                            Boot and recovery errors can also damage the cipher. 
                            Sorry about that, but doing so is entirely at your own risk.


--------------------------------------------------------------------------------------------------
                            
                                  2. EXPLANATION OF THE SITUATION
2.1 HOW DID THIS HAPPEN

The security of your IT perimeter has been compromised (it's not perfect at all). 
We encrypted your workstations and servers to make the fact of the intrusion visible and to prevent you from hiding critical data leaks.
We spent a lot of time researching and finding out the most important directories of your business, your weak points. 
We have already downloaded a huge amount of critical data and analyzed it. Now its fate is up to you, it will either be deleted or sold, or shared with the media.

2.2 VALUABLE DATA WE USUALLY STEAL:
                            - Databases, legal documents, personal information.
                            - Audit reports.
                            - Any financial documents (Statements, invoices, accounting, transfers etc.).
                            - Work files and corporate correspondence.
                            - Any backups.
			    - Confidential documents.
2.3 TO DO LIST (best practies)
                            - Contact us as soon as possible.
                            - Contact us only in our live chat, otherwise you can run into scammers.
                            - Purchase our decryption tool and decrypt your files. There is no other way to do this.
                            - Realize that dealing with us is the shortest way to success and secrecy.
                            - Give up the idea of using decryption help programs, otherwise you will destroy the system permanently.
                            - Avoid any third-party negotiators and recovery groups. They can become the source of leaks.

--------------------------------------------------------------------------------------------------

                                  3. POSSIBLE DECISIONS
3.1 NOT MAKING THE DEAL
                            - After 4 days starting tomorrow your leaked data will be Disclosed or sold.
                            - We will also send the data to all interested supervisory organizations and the media.
                            - Decryption key will be deleted permanently and recovery will be impossible.
                            - Losses from the situation can be measured based on your annual budget.

3.2 MAKING THE WIN-WIN DEAL
                            - You will get the only working Decryption Tool and the how-to-use Manual. 
                            - You will get our guarantees (with log provided) of non-recovarable deletion of all your leaked data.
                            - You will get our guarantees of secrecy and removal of all traces related to the deal in the Internet. 
                            - You will get our security report on how to fix your security breaches.
                    
--------------------------------------------------------------------------------------------------

                                  4. EVIDENCE OF THE LEAKAGE

                			In our live chat
http://p2tn23lt5zpzzyo4bmnpwgbmxhnifggk5ioizmmaeuz4n2bcyv2q44yd.onion/?Url=[snip]
--------------------------------------------------------------------------------------------------

                                  5. HOW TO CONTACT US

5.1 Download and install TOR Browser https://torproject.org
5.2 Go to our live-chat website at http://p2tn23lt5zpzzyo4bmnpwgbmxhnifggk5ioizmmaeuz4n2bcyv2q44yd.onion/?Url=[snip]
5.3 You can request ftp server access in our live chat to review leaked data samples. 
5.4 In case TOR Browser is restricted in your area use VPN services.
5.5 All leaked Data samples will be Disclosed in 4 Days if you remain silent.
5.6 Your Decryption keys will be permanently destroyed at the moment the leaked Data is Disclosed.

--------------------------------------------------------------------------------------------------

                                  6. RESPONSIBILITY

6.1 Breaking critical points of this offer will cause:
                            - Deletion of your decryption keys.
                            - Immediate sale or complete Disclosure of your leaked data.
                            - Notification of government supervision agencies, your competitors and clients.
--------------------------------------------------------------------------------------------------                            
```
