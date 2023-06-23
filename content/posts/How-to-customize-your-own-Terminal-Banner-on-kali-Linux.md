---
title: "How to Customize Your Own Terminal Banner on Kali Linux"
date: 2023-06-23T22:43:36+05:30
draft: false
description: "custom-terminal-thumbnail"
featuredImage: "/custom-terminal.png"
---
Have you ever used any Kali tool and observed a banner of any sort popping up on the terminal? If so, those are figlets, which are simply ASCII letters. Have you ever thought about how to add a banner to your terminal to have a more personalized Linux terminal like the one shown below: 
![sample-banner](/sample-banner.png "Sample Banner")
<!--more-->
Follow the instructions below to set up the banner so that it will show up anytime you open the terminal: 
## Step 1:
firstly, install the lolcat and figlet packages on your Kali Linux machine. 
### Commands
Install FIGlet on Kali : `$ sudo apt install figlet`

Install Lolcat on Kali : `$ sudo apt install lolcat`

To learn more about lolcat, figlet, and other amusing linux commands, see my articles [(Kali) Linux commands for fun: PART-1](https://witchblue.netlify.app/posts/fun-linux-cmd-1/) and [(Kali) Linux commands for fun: PART-2](https://witchblue.netlify.app/posts/fun-linux-cmd-2/)

## Step 2:
Now use an editor to open and navigate to the end of the configuration file `zshrc`.
### Commands
To open zshrc file: `$ nano ~/.zshrc`
![zshrc-file](/zshrc-file.png "This is how the zshrc file appears when scrolled all the way to the bottom.")

## Step 3:
Finally, all that is required to set up the Custom Terminal Banner on Kali Linux is to add a line of script to this file.
### Commands
Script to be added : `figlet "Message" | lolcat`

Note: substitute any name or title of your choice in instead of the "Message".
![script-added](/script-added.png "Line of Script added to the file, underlined in red.")

Press `CTRL + O`, then `Enter`, and then `CTRL + X` to save and close the file.

## Yo! done with setup
And yep, the setup is complete; thats cool, isn't it? Now anytime you open the terminal, a banner you set up will be seen.
Well, the banner will not appear on the root terminal, so the same procedure must be followed to set the root terminal's custom banner.
![final-look](/final-look.png "The customized terminal's final appearance on Kali Linux")


I hope you follow the instructions and customize your terminal. Happy learning, people!