---
layout : post
title  : Could not locate Gemfile or .bundle/ directory
date   : 2019-02-09,
tags : ["jekyll","error"]
categories : jekyll
---

Jika melihat pesan sperti ini saat melakukan run serve jekyll

{% highlight ruby %}
$ bundle exec jekyll serve
Could not locate Gemfile or .bundle/ directory
{% endhighlight %}

Berati kita tidak punya `Gemfile`di derectory kita. <br>
Jika tidak ada `Gemfile` run jekyll tanpa bundle exec. <br>

{% highlight ruby %}
$ jekyll serve
{% endhighlight %}

#maridiskusi

