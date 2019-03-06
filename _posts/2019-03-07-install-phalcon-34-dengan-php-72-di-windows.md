---
title: Install phalcon 3.4 dengan PHP 7.2 di windows
layout : post
date   :  2018-10-20
tags : ["phalcon", "php"]
categories : php
---


Cara nya sebenarnya cukup mudah asalkan teliti download bahan-bahannya sesuai dengan versinya.

yang pertama kita check dulu di `phpinfo()` dan cari bagian ini :

![]({{site.baseurl}}/images/phpinfo.jpg)

yang perlu diperhatikan adalan versi compiler dan architecture nya.<br>
kita punya `compiler = MSVC15 (Visual C++ 2017)` dan `Architecture = 	x64`

Berati kita cari `phalcon dll` yang di compile dari `VC15` dan untuk windows `64bit`,

Dengan begitu kita perlu download `php-phalchon.dll` sesuai versi di atas.[ Download disini](https://github.com/phalcon/cphalcon/releases).


>download  `phalcon vc15 x64 PHP7.2`.
     Aku sarankan pilih yang versi stable nya jangan yang versi alpha.

Setelah selesai download.

>extract file zipnya pindahkan file `php-phalcon.dll` ke dir extension php. Biasanya di dir `C:/xampp/php/ext/`.

>Jangan lupa menambahkan `extension:php-phalcon.dll` di `php.ini`

>restart apache nya

check lagi di phpinfo apakah sudah berasil apa belum. kalau berhasil seharusnya seperti ini:

![]({{site.baseurl}}/images/phpinfo1.jpg)

Selamat. Semoga juga melihat hal yang sama :).
Kalau suka baca yang versi aslinya [disini](https://phalconphp.com/en/download/windows)

#maridiskusi