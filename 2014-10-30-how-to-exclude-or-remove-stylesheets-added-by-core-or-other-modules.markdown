---
layout: post
title: "How to exclude or remove stylesheets added by core or other modules"
date: 2014-10-30 14:42:52 -0500
comments: true
categories: 
---

In Drupal 8, you can easily remove stylesheets added by core, other modules or themes from your custom theme.

Simply add the following lines to your THEMENAME.info.yml file

```
stylesheets-remove:
  - system.theme.css
  - name-of-another-stylesheet.css
```
