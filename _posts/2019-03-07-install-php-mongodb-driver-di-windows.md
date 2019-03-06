---
title: Install php-mongodb driver di windows
layout: post
date: '2018-10-20'
tags:
- mongodb
- php
categories: php
---

Download bahan-bahannya sesuai dengan versinya.

yang pertama kita check dulu Versi PHP dan PHP build kita :

![]({{site.baseurl}}/images/phpinfo2.jpg)

`Thread safe = true` berati kita punya  PHP Build `Thread safe (TS)` dan PHP versi `7.2`
Download mongodb driver sesuai versi di atas. [ Download disini](https://pecl.php.net/package/mongodb/1.4.3/windows).


>download  `7.2 Thread Safe (TS) x64 `. sesuaikan dengan versi windowsnya (x64 / x86)

Setelah selesai download.

>extract file zipnya pindahkan file `php-mongodb.dll` ke dir extension php. Biasanya di dir `C:/xampp/php/ext/`.

>Jangan lupa menambahkan `extension:php-mongodb.dll` di `php.ini`

>restart apache nya

check lagi di phpinfo apakah sudah berasil apa belum. kalau berhasil seharusnya seperti ini:

![]({{site.baseurl}}/images/phpinfo3.jpg)

Semoga berasil juga  ya  :).

#maridiskusi