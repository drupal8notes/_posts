---
layout: post
title: "How to get the current path in Drupal 8"
date: 2014-10-29 23:26:48 -0500
comments: true
categories: 
---

``` php How to get the current path
$current_path = \Drupal::request()->getRequestUri();
```
