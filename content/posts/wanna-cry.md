---
title: "WANNACRY: The Worst Ransomware Attack in History"
date: 2023-05-25T22:33:26+05:30
draft: false
description: "wanna-cry-thumbnail"
featuredImage: "/wannacry.png"
---
This is all you need to know about WannaCry.

<!--more-->

## 1.What is Randsomware?
A form of malware known as ransomware which encrypts all the data on a device and demands randsom in exchange of the keys for accessing the data. 

To make it easier to understand, it is compared to a real kidnapping, in which the kidnappers take the hostages and demand money or something else at a particular time and place in exchange for their release.

## 2.The origin and working of WannaCry

Wannacry is a ransomware cryptoworm cyber attack that first appeared on May 12 2017, at 07:44 UTC, it continued until May 15 2017 and spread automatically throughout the internet. It targeted computers running Microsoft Windows, encrypted (the conversion of plain text to cypher text) the files on the infected system and demanded payment in cryptocurrency (also known as digital currency). 

The typical encryption methods like RSA used in the attack would take millions of billions of trillions of years to break with present-day technology.

### 2.1 Origin
Microsoft weaknesses were first found by the United States National Security Agency (NSA) in 2013, but instead of reporting them, they were piled until eventually a group of hackers known as the shadowbrokers exposed them in a 2016 hack.

By that time, the payload `Doublepulsar` and the exploit `Eternal Blue` (the two components of wannacry), along with numerous other NSA-developed exploits, had been made public.

However, Microsoft released a patch for the vulnerability in March 2017, two months before WannaCry, but the majority of businesses did not update their systems and were using Windows XP or Server 2003; as a result, they were completely vulnerable to the exploit.

### 2.2 Working
Wannacry's damage has been split into two parts: the ransomware payload, which encrypts the files on the computers, and the worm-like component, which atomatically spread the ransomware to the network's compromised machines by using the tools eternalblue and doublepulsar.

* Doublepulsar:
When the NSA's exploits were exposed, the Wannacry hackers took the opportunity and deployed the doublepulsar tool on Windows-based systems, which functions as a backdoor in security by providing a point of entry for hackers to the system and gain easy access for future attacks.

* EternalBlue:  
The following tasks are carried out by EternalBlue:
If a connection to an unregistered domain cannot be made when WannaCry infects the system, damage begins. Then, if port 445, which is used by the Server Message Block (SMB) communication protocol to allow shared access to printers, serial ports, and other network resources, is open, the exploit spreads to other Windows XP, Windows 7, Windows 8, and Windows 10 systems.

>The unregistered domain: `iuqerfsodp9ifjaposdfjhgosurijfaewrwergwea.com`

![screenshot of the ransom notice found on a compromised computer](/wannacry-note-screenshot.png "screenshot of the ransom notice found on a compromised computer")

## 3.The impact of WannaCry
>According to Cyence, a company that models cyber-risk, the attack caused a $4 billion dollar economic loss.

Wannacry is thought to have infected over 200,000 systems across 150 countries, 70,000 of which were from National Health Service (NHS) hospitals in England and Scotland since they remained running Windows XP. However, the attack had no impact on the NHS in Wales or Northern Ireland.

In an effort to limit the spread of the ransomware, many IT and other businesses, including Nissan Motors, Renault, Telefónica, FedEx, and Deutsche Bahn stopped production at various sites.

## 4.Who was behind WannaCry?
The US Department of Justice and British officials later blamed the WannaCry attack on the `Lazarus group`, a North Korean hacker gang.

### 4.1 The Lazarus Group
![Lazarus group](/lazarus.jpg "the lazarus group")
The Lazarus Group, also known as Guardians of Peace, Whois Team, Hidden Cobra, or Zinc, is a state-sponsored hackers organisation that is under the control of North Korea, says the Federal Bureau of Investigation in the United States. 

According to North Korean defector Kim Kuk-song, it is internally named as the "414 Liaison Office". Therefore, this is a component of the General Bureau of Reconnaissance. The Lazarus Group is not widely known but between 2010 and 2021, they are believed to have been responsible for a large number of cyberattacks.

### 4.2 Motive
The security experts believed that the WannaCry attacker's objective was more political in nature, such as bringing shame to the NSA. However the attackers intent remained a mystery.

## 5.How did it stopped?
WannaCry had if-then statements with an in-built kill switch that is if it fails to connect to the domain; if it can connect, it shuts itself down.

The wannacry sample was tested by British security researcher `Marcus Hutchins` alias MalwareTech using fake files, and on May 12 2017 at 15:03 UTC he discovered that it was attempting to connect to a domain (iuqerfsodp9ifjaposdfjhgosurijfaewrwergwea.com). He not only found the hard-coded URL, but he also spent $10.96 to register the domain, which ultimately prevented the ransomware outbreak. 

It was noted that 2 million devices had been prevented from being infected two days after the domain went live. 



### 5.1 More about Hutchins-The accidental Hero
![Marcus Hutchins](/marcus_hutchins.jpg "Marcus Hutchins")

Hutchins got unwanted attention as a result of all of this, which he did not enjoy, and three months later, in August 2017, the FBI arrested him. Hutchins had created a malware called `Kronos in 2014` that steals bank credentials; he sold this malware to a man he met online by the name of Vinnie K which is still a threat to banks all over the world. 

After a year of trials, he was eventually set free. Despite being given a 10-year prison sentence, his active role in putting an end to wannacry allowed him to stay out of it.

## 6.How to prevent such attacks?
Listed below are a few ways to stop ransomware and other attacks:

- Avoid clicking on links from unknown sources.
- Keep your personal details to yourself. 
- Never utilise unfamiliar external devices, such as USBs or flash drives.
- Maintain devices up-to-date with updates
- Install softwares only from reliable sources.
- When using public Wi-Fi networks, use VPN services.
- Educate employees about the issue
- Backup the data on a regular basis.
- Preparing a plan in case of ransomware attack

## 7.Conclusion
Thus, this is all about WannaCry the most devastating historical ransomware attack.


Happy reading, and I hope this article is helpful...🐾