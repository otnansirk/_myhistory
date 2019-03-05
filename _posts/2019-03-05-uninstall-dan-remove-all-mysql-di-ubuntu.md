---
title: Uninstall dan remove all mysql di ubuntu
layout: post
date: '2019-03-05'
category: ubuntu
cat-image: cat-ubuntu.jpg
tags:
- ubuntu
- bash
---

###### Kita akan meremove dan mencoba menginstall kembali mysql.  kita lihat step by stepnya ya.

### Remove Mysql

> sudo apt-get remove --purge mysql*

> sudo apt-get purge mysql*

> sudo apt-get autoremove

> sudo apt-get autoclean

> sudo apt-get remove dbconfig-mysql

> sudo apt-get dist-upgrade

<br><br>
### Install mysql last version.

> sudo apt-get install mysql-server

<br><br>
### Install mysql 5.6

##### update sofware ditambahkan ke repositori 14.04

>deb http://archive.ubuntu.com/ubuntu trusty main

##### Install Mysql client

>sudo apt install mysql-server-5.6

##### Install Mysql client

>sudo apt install mysql-client-5.6

semoga bermanfaat.

#maridiskusi