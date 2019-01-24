---
layout : post
title  : Menghilangkan watermark 000webhost.com
date   : 2019-01-25,
tags : ["trick","javascript"]
categories : trick
---


Cara menghilangkannya sebenernya cukup simple. kita hanya perlu tahu dimana kode 000webhost.com itu berada. 
coba saja buka web kalian yang memiliki watermark 000webhost `lalu ctrl + u` (Di chrome windows). Cari tagnya 000webhost kalau sudah
Edit file index dan letakkan kode di bawah ini. di paling bawah bagian atas tag `</body>`.

``` 
$(document).ready(function(){
   $('body').find('Tag yang ingin di hapus letakkan disini').remove();
});
```

Dan pada saat menulis Dokumentasi ini. tag www.000webhost.com memiliki `alt="www.000webhost.com"`. 
maka script nya akan menjadi seperti ini.

``` 
$(document).ready(function(){
   $('body').find('[alt="www.000webhost.com"]').remove();
});
```

Jangan ragu untuk bertanya tentang hal lain. :D </br>
#maridiskusi


