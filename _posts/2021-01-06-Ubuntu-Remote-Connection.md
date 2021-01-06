---
layout:     post
title:      Ubuntu Remote Connection
subtitle:   How to use your local terminal to control Ubuntu?
date:       2021-01-06
author:     Jimeng
header-img: img/southeast_view.jpg
catalog: true
tags:
    - Ubuntu, Linux
---

## 1. Update the system using the apt command or apt-get command:
    $ sudo apt update
    $ sudo apt upgrade

## 2. Ubuntu Linux install OpenSSH server on Ubuntu Linux
    $ sudo apt install openssh-server


## 3. Verify that ssh service running
Type the following systemctl command:
    
    $ sudo systemctl status ssh


Check to confirm that OpenSSH server running on Ubuntu. If not running enable the ssh server and start it as follows by typing the systemctl command:
    
    $ sudo systemctl enable ssh
    $ sudo systemctl start ssh


## 4. Configure firewall and open port 22
You must configure the Ubuntu Linux firewall called ufw. Here is how open or allow port 22 when using ufw on Ubuntu: [1]

    $ sudo ufw allow ssh
    $ sudo ufw enable
    $ sudo ufw status


## 5. Test connection
Now you can login from your desktop computer powered by Linux, *BSD, macOS, MS-Windows (putty client) or Unix-like system using the ssh command: [2]
    
    $ ifconfigure                 # check your ip address in Ubuntu
    $ ping server-ip
    $ ssh user_name@server-ip

**PS: Installing OpenSSH from the Settings UI on Windows 10** [3]

OpenSSH client and server are installable features of Windows 10.

To install OpenSSH, start Settings then go to Apps > Apps and Features > Manage Optional Features.

Scan this list to see if OpenSSH client is already installed. If not, then at the top of the page select "Add a feature", then:

- To install the OpenSSH client, locate "OpenSSH Client", then click "Install".
- To install the OpenSSH server, locate "OpenSSH Server", then click "Install".


## Reference
[1] https://www.cyberciti.biz/faq/ubuntu-linux-install-openssh-server/

[2] https://www.bilibili.com/video/BV1y7411d76V?p=12

[3] https://docs.microsoft.com/en-us/windows-server/administration/openssh/openssh_install_firstuse#:~:text=To%20install%20OpenSSH%2C%20start%20Settings,%2C%20then%20click%20%22Install%22.
