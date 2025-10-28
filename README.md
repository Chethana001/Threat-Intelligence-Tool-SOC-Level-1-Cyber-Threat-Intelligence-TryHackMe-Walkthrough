# Threat-Intelligence-Tool-SOC-Level-1-Cyber-Threat-Intelligence-TryHackMe-Walkthrough
Threat Intelligence Tools— SOC Level 1 -Cyber Threat Intelligence — TryHackMe Walkthrough
## Task one : Room Outline
This room will cover the concepts of Threat Intelligence and various open-source tools that are useful. The learning objectives include:

* Understanding the basics of threat intelligence & its classifications.
* Using UrlScan.io to scan for malicious URLs.
* Using Abuse.ch to track malware and botnet indicators.
* Investigate phishing emails using PhishTool
* Using Cisco's Talos Intelligence platform for intel gathering.

## Task two : Threat Intelligence
### What is Threat Intelligence?

It’s basically detective work for cyberattacks.
You collect clues (data) about bad guys trying to hack companies or governments, then figure out who they are, why they’re coming, and how to stop them.

### To stop the bad guys, ask 4 simple questions

1. Who’s trying to break in?
(A hacker group? A country? A disgruntled ex-employee?)\
2. Why do they want in?
(Steal money? Spy? Cause chaos? Ransom?)\
3. What tools and skills do they have?
(Are they using sneaky phishing emails? Super advanced malware?)\
4. What clues should we look for?
(Weird login attempts? Strange files? Warning signs on our systems?)

### 4 Types of Threat Intel

<img width="966" height="378" alt="image" src="https://github.com/user-attachments/assets/dbb7f1a5-1a3a-4b98-a260-f6dcf4a956e1" />
## Task three : UrlScan.io
### What is urlscan.io?
It’s a free online tool that acts like a safe robot browser.
You give it a web link (URL), and it visits the site for you in a secure sandbox (like a locked room). Then it records everything the site does—without risking your own computer.

### Why is this useful?

* Spot phishing sites (fake bank logins, etc.)
* Check if a link is safe before clicking
* See if a site is spying or loading malware
* Help security teams investigate attacks

### Scan Results


<img width="972" height="579" alt="image" src="https://github.com/user-attachments/assets/541826e6-77da-4c20-b37d-c677697f0a22" />

### Scenario


You have been tasked to perform a scan on TryHackMe's domain. The results obtained are displayed in the image below. Use the details on the image to answer the questions:
<img width="1292" height="1004" alt="image" src="https://github.com/user-attachments/assets/f4179200-ecc6-442c-ac1e-aee8b11f071c" />


* What was TryHackMe's Cisco Umbrella Rank based on the screenshot? : 345612
* How many domains did UrlScan.io identify on the screenshot? : 13
* What was the main domain registrar listed on the screenshot? : NAMECHEAP INC
* What was the main IP address identified for TryHackMe on the screenshot? : 2606:4700:10::ac43:1b0a

## Task Four : Abuse.ch

Abuse.ch as Switzerland’s free cyber-crime lab 
Run by smart folks at a university, it’s like a public bounty board for tracking digital bad guys.
They built 5 free tools (platforms) to share clues about malware and hacker hideouts.

### Abuse.ch Platforms

<img width="973" height="453" alt="image" src="https://github.com/user-attachments/assets/44cb0da8-30e3-45cf-94f5-63a411d2dab9" />

### Malware Bazaar
Malware Bazaar, run by the Swiss Abuse.ch project, is a free, all-in-one malware collection and analysis database where security analysts can upload real malware samples via a simple browser drag-and-drop or automated API to help build a global intelligence library; once uploaded, samples are scanned, tagged, and made publicly searchable. It also supports powerful “malware hunting” by letting users set up real-time alerts based on specific criteria like tags (e.g., “ransomware”), YARA rules, ClamAV signatures, or antivirus vendor detections (e.g., Microsoft, Kaspersky), so you’re instantly notified when matching threats appear—making it an essential tool for researchers, incident responders, and defenders to study, share, and block the latest malware before it spreads.

### Feodo Tracker

Feodo Tracker is like a "Wanted Posters" wall for the boss computers that control zombie armies (botnets).
These botnets are called Dridex, Emotet, TrickBot, QakBot, and BazarLoader — they steal bank logins, spam emails, and lock files for ransom

### SSL Blacklist
imagine SSL Blacklist as the “Fake Padlock Police” 
You know how websites show a little lock saying “secure”? Hackers fake that lock to trick you.


SSL Blacklist says:

“We caught the crooks using fake SSL certificates and secret handshakes (JA3 fingerprints) to talk to their botnets. Here’s the naughty list — block them!”

### URLhaus
URLhaus as the “Do Not Click” list for the internet 
It’s a giant, free database of bad links that spread like to hand out viruses — think fake software updates, phishing emails, or drive-by downloads.

### ThreatFox
imagine ThreatFox as the “Crime Scene Evidence Board” 
It’s where security pros dump, search, and grab IOCs — the digital fingerprints left by malware (like IP addresses, domains, file hashes).



