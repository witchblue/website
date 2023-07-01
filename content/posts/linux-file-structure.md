---
title: "Linux File Structure"
date: 2023-06-15T21:38:40+05:30
draft: false
description: "linux-file-structure-thumbnail"
featuredImage: "/linux-file-struct.png"
---
Do you frequently lose track of where you placed your clothes, keys, and other stuff? Isn't it more difficult to track them down when you need them? The majority of us arrange them accordingly, putting keys on a desk or hooks and clothes in closets. Similar to how our computer's operating system organizes the files in the structure, making them simple to access when necessary. In this article, I will explain the Linux file structure in a simple way.
<!--more-->
## File Hierarchy Structure (FHS) in Linux
The Filesystem Hierarchy Standard (FHS), often known as the Linux File Hierarchy Structure (Linux FHS), describes how the Linux operating system's directories and contents are organized.
![linux-file-structure](/linux-filesystem-hierarchy.png "File Hierarchy Structure (FHS) in Linux | Credit: tecadmin.net")
The following are a few important directories:
### / (root)

As shown in the image above, the forward slash (/) stands in for the root directory where the other directories are maintained.
- Every single directory or file begins with the root directory.
- Within this directory, only the root user is permitted to write.

Example: /home/file.txt
![root-linux-directory](/root.png "root-linux-directory")
### /home
The home directory contains all of the user's folders, such as user's home directories, personal files, and so on.
- It is the initial current directory that appears when you launch a terminal

Example: /home/blue, /home/kali
![home-linux-directory](/home.png "home-linux-directory")

### /usr
All of the executable files, libraries, and source code for the majority of the system programs can be found in "/usr." Because of this, the majority of the files therein are read-only (for the normal user).
![usr-linux-directory](/usr.png "usr-linux-directory")
- Basic user commands can be found in "/usr/bin."
![usr-bin-linux-directory](/usr-bin.png "usr-bin-linux-directory")
- Additional commands for the administrator can be found in "/usr/sbin."
![usr-sbin-linux-directory](/usr-sbin.png "usr-sbin-linux-directory")
- The system libraries are located in "/usr/lib."
![usr-lib-linux-directory](/usr-lib.png "usr-lib-linux-directory")
- '/usr/share' contains information that is common to all libraries, such as the text of the man page in '/usr/share/man'.
![usr-share-man-lib-linux-directory](/usr-share-man.png "usr-share-man-lib-linux-directory")

### /etc
It contains all of the configuration files necessary for the system that are specific to each program.
- The shell scripts needed to start/stop specific programs are also included here.

Examples include /etc/logrotate.conf and /etc/resolv.conf.
![etc-linux-directory](/etc.png "etc-linux-directory")

### /root
The /root directory serves as the super user's home directory. This directory is different from /(root).
![/root-linux-directory](/root-root.png "/root-linux-directory")

### /opt
It is referred to as the system's optional third-party software and contains add-on apps from various vendors.
Applications for add-ons ought to be installed in the /opt/ or /opt/subdirectory.
![opt-linux-directory](/opt.png "opt-linux-directory")

### /lib
Contains every necessary library file that the system uses for the binaries in /bin/ and /sbin/.
- Either ld* or lib*.so.* are used as library filenames.
Example: ld-2.11.1.so, libncurses.so.5.7
![lib-linux-directory](/lib.png "lib-linux-directory")

### /boot 
All of the files required for Linux to boot, as well as grub, a little program that allows to select the OS and boot it.
Example: vmlinuz-2.6.32-24-generic , initrd.img-2.6.32-24-generic
![boot-linux-directory](/boot.png "boot-linux-directory")

### /bin
It stores binaries, which are executable files of several basic shell operations like as ls, cp, cd, and so on.
![bin-linux-directory](/bin.png "bin-linux-directory")

### /sbin
Similar to the /bin directory but only containing specific commands that the root user can execute 
Example: swapon, ifconfig, fdisk, reboot, and iptables
![sbin-linux-directory](/sbin.png "sbin-linux-directory")

### /var
Var, short for variable, is the location where programs keep track of runtime data including user tracking, system logging, caches, and other files that system programs produce and manage.
For instance, you can inspect the contents of the file under /var/log/wtmp to see your Linux system's login history.
![var-log-linux-directory](/var-log.png "var-log-linux-directory")

### /media
When a removable device is connected, such as a USB disc, SD card, or DVD, a directory is automatically established under the /media directory for them, from which the content of the removable media can be accessed.
![media-linux-directory](/media.png "media-linux-directory")

### /mnt 
Similar to the /media directory, however system administrators use mnt to specifically mount filesystems rather than automatically mounting removable media.
![mnt-linux-directory](/mnt.png "mnt-linux-directory")

### /tmp
Temporary files created by the system and users are kept in this directory.
When the system reboots, the files in this directory are removed.
![tmp-linux-directory](/tmp.png "tmp-linux-directory")

Other essential directories are the /run directory, which holds runtime data for processes that are actively operating on the system, /srv directory directs users to the location of data files for a certain service, such as FTP, WWW, or CVS and The files in the /dev directory represent the devices that are connected to the local system.

One can quickly browse Linux by learning the purpose of each directory.