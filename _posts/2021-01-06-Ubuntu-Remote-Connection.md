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
You must configure the Ubuntu Linux firewall called ufw. Here is how open or allow port 22 when using ufw on Ubuntu:

    $ sudo ufw allow ssh
    $ sudo ufw enable
    $ sudo ufw status


## 5. Test it
Now you can login from your desktop computer powered by Linux, *BSD, macOS, MS-Windows (putty client) or Unix-like system using the ssh command:
    
    $ ifconfigure                 # check your ip address in Ubuntu
    $ ping server-ip
    $ ssh user_name@server-ip


## 6. Reference
[1] https://www.cyberciti.biz/faq/ubuntu-linux-install-openssh-server/

[2] https://www.bilibili.com/video/BV1y7411d76V?p=12
