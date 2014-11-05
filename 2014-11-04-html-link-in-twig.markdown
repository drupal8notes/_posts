---
layout: post
title: "HTML link in Twig"
date: 2014-11-04 21:45:59 -0800
comments: true
categories: 
---

In Drupal 7, you could use the `array('html' => TRUE)` parameter to make an HTML link. Here's how to do it in Twig.

{% codeblock %}
{% raw %}
{{ link(title, url.setOption('html', true)) }}
{% endraw %}
{% endcodeblock %}

Note that url should be an instance of `\Drupal\Core\Url`.
