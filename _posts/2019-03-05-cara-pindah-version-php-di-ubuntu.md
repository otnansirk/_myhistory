---
title: Cara pindah version php di ubuntu
layout: post
date: '2019-03-05 15:30:00'
category: trick
tags: [ubuntu, bash]
---

Jika kita udah menginstall php dengan lebih dari satu version misal contoh kita punya `php7.2` dan `php5.6` . kita bisa pindah-pindah versi php sesuai dengan yang kita inginkan. <br> 
mungkin command ini bisa membantumu.

misal kita mau pindah dari php7.2 ke 5.6 
```
sudo a2dismod php7.2
sudo a2enmod php5.6
sudo update-alternatives --set php /usr/bin/php5.6
sudo service apache2 restart
```

atau sebaliknya dari php5.6 ke 7.2
```
sudo a2dismod php5.6
sudo a2enmod php7.2
sudo update-alternatives --set php /usr/bin/php7.2
sudo service apache2 restart
```

sedikit cara ini semoga membantu. 

#maridiskisi