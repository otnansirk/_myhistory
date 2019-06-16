---
title: Php Mengatasi Curl_init() Error Ubuntu
layout: post
date: '2018-10-20'
tags:
- php
categories: php
cat-image: cat-php.jpg
---

Jika mengalami error curl_init() jangan kawatir coba check di `php.ini` apakah
curl ini sudah di install atau belum. bisa juga dengan.

{% highlight php %}
sudo php -m | grep "curl"
{% endhighlight %}

Jika response dari perintah di atas kosong, berati curl_init tidak diload oleh php.
dan ini yang menyebabkan error `Fatal error: Call to undefined function curl_init() in …`

Berati kita perlu menginstallnya dengan.

{% highlight php %}
sudo apt-get install php5-curl
{% endhighlight %}

Jika ada konfirmasi (y/n), pilih y untuk lanjut install

Setelah itu jangan lupa untuk merestart apache nya.

{% highlight php %}
sudo service apache2 restart
{% endhighlight %}