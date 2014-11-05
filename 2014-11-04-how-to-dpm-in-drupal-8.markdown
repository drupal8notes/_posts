---
layout: post
title: "How to dpm in Drupal 8"
date: 2014-11-04 21:19:22 -0800
comments: true
categories: 
---

Looks like `dpm()` is broken right now in devel. It gives you a WSOD.

Here's some alternatives with the devel module enabled:

#### 1. Krumo

``` php
krumo($variables);
```

#### 2. Kint
[Kint](http://raveren.github.io/kint/) is a great alternative to Krumo.

``` php
kint($variables);
```

#### 2.Dump for Twig
Inside Twig template you can:

{% codeblock %}
{% raw %}
{{ dump() }}
{% endraw %}
{% endcodeblock %}

