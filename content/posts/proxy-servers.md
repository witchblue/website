---
title: "Proxy Servers"
date: 2023-11-25T22:25:48+05:30
draft: false
description: "proxy-servers-thumbnail"
featuredImage: "/proxy-servers.png"
categories: ["kali" , "Tutorial"]
author: "Witchblue"
---
Would you like to surf the web in absolute anonymity? or get over network limitations? If Yes, you will now learn how to set up and utilize Proxy Chains from this tutorial.
<!--more-->

## Proxychains??

Proxychains is a command-line utility that lets you route network traffic across numerous proxy servers. It seeks to increase anonymity and overcome network limitations.

## Proxychains vs VPN

Proxychains is intended to provide greater anonymity than a traditional VPN.
When you utilize a VPN, there is usually only one proxy server between you and the destination. The VPN software encrypts your data before sending it to the VPN server, which serves as a proxy on your behalf.

However, utilizing a VPN leaves a trail of your activities on the proxy server, which could jeopardize your anonymity.

Proxychains takes a different approach: it requires every TCP communication from your system to pass through a series of different proxies before reaching the destination host.
Chaining proxies provides better privacy and reduces the chance of leaving traces.

## Uses

- Proxychains shine when complete anonymity is required for tasks like as pen testing or data sniffing.
- It assures that no traces of your system are left behind, making it an invaluable resource for cybersecurity professionals.

## Installation process
Follow the commands below to install, configure and utilize the proxychains tool:
    
 Step 1: `sudo apt install proxychains` to install the proxychains tool
    ![Proxychains Installation ](/proxychains-install.png "Proxychains Installation")
    
 Step 2: `sudo nano /etc/proxychains.conf` to open the proxychains configuration file
    ![Proxychains.conf ](/proxychains.conf.png "/etc/proxychains.conf file")

 Step 3: Uncomment dynamic chains and comment strict chains as shown in the picture below, and if you want to boost anonymity, add proxy servers that are freely available online, such as `https://vpnoverview.com/privacy/anonymous-browsing/free-proxy-servers/`.
    ![uncomment ](/uncomment.png "Changes in file contents")
    ![proxyserver ](/proxyserver.png "In the bottom of the same file, you can add proxy servers")

 Step 4: One by one, hit `Ctrl + o` , `Enter`, `Ctrl + x` to save the contents of the file.     

 Step 5: `sudo apt install tor` to install tor (Any error while installing tor then do this -- **apt-get update && apt-cache search tor** ) 
 ![tor-installation](/tor-installation.png "Installing tor")

 Step 6: `sudo service tor start` to start the tor service
 ![start-tor](/start-tor.png "Starting the tor service")

 Step 7: `sevice tor status` to check whether the tor service is running or not
 ![tor-status](/tor-status.png "Checking tor status")

 Step 8: Finally, after the installation and configuration process is completed, use the command `proxychains firefox` or any other program to utilise the proxychains. I opened the Firefox browser with proxychains and then headed to the DNS leak test website to run the dns leak test which is a security flaw that allows DNS requests to be revealed to ISP DNS servers, despite the use of a VPN service to attempt to conceal them. As You can see that my location has now changed from INDIA to POLAND, and the good thing is that proxychains constantly changing my IP address in a dynamic way to ensure good anonymity.

 ![dns-leak-test](/dns-leak-test.png "dns-leak-test")

## Conclusion
Setting up proxychains is easy, and it is a simple approach to dynamically increase anonymity online.

Meet you soon in my next article; till then, take care and have fun, peeps.






