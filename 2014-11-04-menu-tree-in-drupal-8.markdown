---
layout: post
title: "menu_tree() in Drupal 8"
date: 2014-11-04 21:39:29 -0800
comments: true
categories: 
---
In Drupal 7, you can use menu_tree to load the entire menu tree.

Here's how to do it in Drupal 8:

``` php
// Format and add main menu to theme.
$menu = \Drupal::menuTree()->load('main', new MenuTreeParameters());
$variables['main_menu'] = \Drupal::menuTree()->build($menu);
```
