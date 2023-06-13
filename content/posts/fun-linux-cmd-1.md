---
title: "(Kali) Linux commands for fun: PART-1"
date: 2023-06-11T22:30:01+05:30
draft: false
description: "linux-fun-thumbnail"
featuredImage: "/linux-fun.png"
---
Typically, the powerhouse for its user and sysadmins is the terminal. Linux, however, is more than just a lot of laborious effort.  There is a lot of excellent open source software available, but some of it was created purely for enjoyment. When you wish a smile, play with these on your own.
<!--more-->

## Steam locomotive (sl)
The command `"sl"` stands for steam locomotive, and when it is executed, a stream locomotive moves across the terminal. Its objective is to be laughable if someone mistypes the `ls` command.

### Commands
Install Steam Locomotive on Kali : `$ sudo apt install sl`

To run sl: `$ sl`
![sl](/sl.png "Stream locomotive")

## Lolcat
Lolcat is a package that adds a rainbow colouring effect to text displayed on consoles. It can also be piped with other command's output to add a rainbow tint to the result. 

### Commands
Install Lolcat on Kali : `$ sudo apt install lolcat`

To run lolcat: `$ ls | lolcat` 
Note: This is just an example; any command can be used to pipe with lolcat.
![lolcat](/lolcat.png "Lolcat piped with the output of ls command")

## FIGlet and banner
The FIGlet and banner commands allow you to make simple ASCII text banners. With the use usual text, it transforms the provided data into a banner.

### Commands
Install FIGlet on Kali : `$ sudo apt install figlet`

To run FIGlet: `$ figlet "The Text"` 
![FIGlet](/figlet.png "FIGlet")

Install banner on Kali : `$ sudo apt install banner`

To run banner: `$ banner "The Text"` 
![banner](/banner.png "banner")

## FIGlet fonts with lolcat
With lolcat, you can also use figlet and banner as well. Here, I'll show you how to use lolcat with figlet and its beautiful fonts.

### Commands
Lolcat with figlet: `$ figlet "witchblue" | lolcat`
![lolcat-figlet](/fig-lol.png "Lolcat with figlet")

To view figlet fonts : `$ showfigfonts`
![showfigfonts](/figfonts.png "showfigfonts")

Figfonts and lolcat combo: `$ figlet -f slant  "witchblue" | lolcat`
![combo](/fig-lol-font.png "Figfonts and lolcat combo")


To explore all the options and iterations, make sure you explore the man pages of each command. I really hope you enjoy experimenting with these fun commands...
