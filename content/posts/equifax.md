---
title: "Equifax Data Breach"
date: 2023-08-11T17:25:06+05:30
draft: false
description: "equifax-thumbnail"
featuredImage: "/equifax.png"
categories: ["Case Study"]
---
Have you recently thought about what an organization might face if the software it is using to construct its web applications is out of date? then take a look at this article, which discusses the 2017 data breach at the consumer credit reporting company "Equifax." 
<!--more-->
## Equifax
Equifax founded in 1899 and with its headquarters in Atlanta, Georgia; is one of the three main `US credit reporting agencies`, together with Experian and Transunion, and it has access to information on millions of customers and companies around the world. 

In addition to determining how difficult it will be for a consumer to receive loans, Equifax also sells consumer and business credit reports to commercials including banks, insurance companies, and healthcare providers. 
## Data breach
### The vulnerability and its fix
The Equifax website is developed on software known as apache struts, a popular framework for developing program that enable companies in managing big amounts of data online. 

The Apache foundation, which is in charge of struts, reported the presence of a serious software vulnerability in March of 2017 that they called `CVE-2017-5638`. 

Additionally, the Apache Foundation simultaneously with its announcement of its existence provided a fix for it. The repair could take some time because it needs manually updating and rebuilding each app that utilizes the Struts framework, which could number in the dozens or hundreds for a single company.

### CVE-2017-5638 aka Apache Struts2 Remote Code Execution
The Apache Struts web application framework includes the Jakarta Multipart parser, which is used to manage file uploads in web applications. Through HTTP requests, it enables users to upload files, which the server then processes. 

The `Jakarta Multipart parser` is vulnerable, according to Apache. An exception is raised if the Content-Type header has an incorrect value. The user is shown the error via the exception. Through the use of the Content-Type header, an attacker can use this flaw to move from the data scope to the execution scope.

Consider the following situation to gain more understanding, we have filled out web forms countless times to place orders, sign up for accounts, contact customer service, and all kinds of other things. However, a flaw in how struts handles data entered into these forms allows for `remote code execution`, a type of hack that allows for the sending of malicious code to the servers that hold the data. 

With this vulnerability, hackers might cause an error and then force the server to execute the embedded commands while it was attempting to find out what the mistake was. 

Normally, programmers would defend against this by having the server examine what you're submitting to make sure it's not computer code. This bug is quite serious.  

### Skipped the update??
Sadly, `Equifax failed to notice the vulnerability and update`, which later impacted a number of negative effects. However, the attack on Equifax's system using this vulnerability started in mid-May, two months after it was discovered. 

## The impact of Data breach
The 2017 Equifax data breach had a major effect on the firm as well as millions of people whose personal and financial information was exposed. Some of the main effects of the Equifax data leak include:
- `Massive Data Breach:` The breach resulted in the exposure of 147 million people's personal data, including names, social security numbers, birth dates, addresses, and credit card information. 

- `Identity theft and fraud:` Because of the exposed data, fraudsters have been able to commit a variety of identity theft and financial fraud schemes. This includes getting loans, creating new accounts, and carrying out unauthorized transactions using stolen data.

- `Legal and regulatory consequences:` Due to government investigations and consumer lawsuits regarding the improper handling of sensitive data, the company faced large penalties and legal expenses.

- `Reputational Damage:` The hack significantly harmed Equifax's reputation and eroded public trust. Customers, investors, and business partners began to doubt the company's capacity to protect sensitive information as a result of the incident, which exposed the company's weak security procedures and response tactics.

- `Financial Losses:` Due to the breach, Equifax experienced financial losses, which included remediation costs, litigation costs, fines from the government, and customer compensation. 

- `Consumer Dissatisfaction:` Affected individuals experienced inconvenience and irritation as a result of the breach's consequences. Many had to keep an eye on their credit reports, freeze their credit files, and take further security measures to safeguard their identities.


## Who was behind it?
Although there has been no more proof that China used the data from the attack, `the United States Department of Justice` stated on February 10, 2020 that it has indicted four members of the Chinese military on nine crimes relating to the hack. The Chinese government has denied that the four accused were involved in the cyberattack.

## Criticism
Due to a number of circumstances, Equifax received a `lot of backlash` following its data breach. The business received criticism for taking so long to identify and disclose the breach and for not notifying the impacted customers immediately. 

Millions of people's sensitive personal and financial information were exposed in the hack, which was of such a size that it prompted questions about Equifax's data protection policies and security safeguards. The way the business handled contacting those who were affected as well as the efficiency of their cybersecurity procedures to stop such attacks were also criticized. 

The hack highlighted the significance of strong cybersecurity procedures and open communication in protecting private information and upholding public confidence.
## How to prevent such attacks?
Organizations may put the following precautions into place to stop data breaches and cyberattacks like the one that Equifax experienced:

1. `Use Strong Security Practices:` To safeguard systems and networks from unauthorized access, use security measures like firewalls, intrusion detection systems, and antivirus software.

2. `Regular Software Updates:` To address vulnerabilities that attackers may exploit, keep all software, including operating systems and apps, up to date with the most recent security patches.

3. `Strong Authentication:` Use multi-factor authentication (MFA) to ensure only authorised users have access to important systems and data.

4. `Data Encryption:` To prevent unauthorized access even in the event of a breach, encrypt sensitive data both at rest and in transit.

5. `Employee Training:` Regularly educate staff members on cybersecurity to increase knowledge of phishing scams, social engineering, and safe online conduct.

6. `Access Control:` Establish a need-to-know basis for limiting access to vital systems and data. Restrict access rights for former workers and contractors on a regular basis.

7. `Incident Response Plan:` Create and keep an incident response plan up to date in order to promptly identify, contain, and lessen the effects of possible breaches.

8. `Vendor Security:` Verify the security procedures in place at third-party vendors and partners who have access to your systems or data.

9. `Regular Audits:` To find flaws and vulnerabilities that require attention, conduct routine security audits and penetration testing.

10. `Data Retention:` Only keep the minimum amount of sensitive client information on file, and securely delete any information that is no longer required.

11. `Legal and Regulatory Compliance:` Keep current on pertinent laws and rules to guarantee adherence to data protection requirements.

12. `Transparent Communication:` To exhibit transparency and uphold confidence, notify impacted parties, clients, and regulators as soon as possible in the event of a breach.

Organizations can improve their entire cybersecurity posture by employing these preventive measures, which greatly minimize the likelihood of data breaches and cyberattacks.

## Conclusion
So the whole story revolves on the Equifax data breach, a cyber attack that caused such a severe data leakage simply because the company neglected to upgrade the software it used for its online data management. And stay tuned for more case studies, tutorials, and so much more. 

Happy reading, everyone!
