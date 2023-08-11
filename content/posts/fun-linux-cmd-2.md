---
title: "(Kali) Linux commands for fun: PART-2"
date: 2023-06-17T17:58:51+05:30
draft: false
description: "linux-fun-thumbnail"
featuredImage: "/linux-fun2.png"
categories: ["Kali"]
---
This is the second part of the "linux commands for fun" series. 
<!--more-->

## Cowsay
Cowsay is a simple and funny program in which the cow accepts a text string and generates a ASCII art representation of a cow talking. It serves no purpose other than to give the terminal some interesting style. 

### Commands
Install Cowsay on Kali : `$ sudo apt install cowsay`

To run cowsay: `$ cowsay "I love Linux"`
![cow-saying-it-loves-Linux](/cowsay.png "Cow saying it loves Linux")

## cbonsai
"cbonsai" is a command-line interface (CLI) tool for creating visually beautiful ASCII art representations of bonsai trees at random. It attempts to deliver a fun and aesthetic experience by developing virtual bonsai trees that can be displayed on the terminal.

### Commands
Install cbonsai on Kali : `$ sudo apt install lolcat`

To run cbonsai: `$ cbonsai` 
![cbonsai](/cbonsai.png "Basic bonsai illustation")

Few more cbonsai Command Examples
1. Generate a bonsai in live mode: `cbonsai -l`
2. Generate a bonsai in infinite mode: `cbonsai -i`
3. Append a message to the bonsai: `cbonsai -m "message"`
4. Display extra information about the bonsai: `cbonsai -v`
5. Display cbonsai help: `cbonsai -h`

## Fireplace (aafire)
Use the aafire command to play an ASCII-art version of a fireplace animation, warming both the heart and the terminal.

### Commands
Install Fireplace on Kali : `$  sudo apt install libaa-bin`

To run Fireplace: `$ aafire` 
![aafire](/aafire.png "aafire")


Similarly to part 1, make sure to read through the man pages of each command to explore all the options and iterations. I truly hope you have fun playing around with these entertaining commands.