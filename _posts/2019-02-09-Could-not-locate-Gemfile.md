---
layout : post
title  : Could not locate Gemfile or .bundle/ directory
date   : 2019-02-09,
tags : ["jekyll","error"]
categories : jekyll
---

Jika mengalami error ERROR: Failed to build gem native extension saat menjalankan gem install jekyll bundler ? Mungkin kita belum menginstall ruby-dev.

Coba install ruby-dev dulu dengan command. 
{% highlight ruby %} 
  $ apt-get install ruby-dev 
{% endhighlight %}

setelah itu coba kita lakukan lagi install jekyll bundler dengan command. 
{% highlight ruby %} 
  $ gem install jekyll bundler 
{% endhighlight %}

#maridiskusi

