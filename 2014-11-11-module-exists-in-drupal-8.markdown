---
layout: post
title: "module_exists in Drupal 8"
date: 2014-11-11 12:12:13 -0500
comments: true
categories: 
---
How to check if a module is enabled in Drupal 8:

```
\Drupal::moduleHandler()->moduleExists('search')
```
