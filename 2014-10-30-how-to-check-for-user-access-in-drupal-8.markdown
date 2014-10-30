---
layout: post
title: "How to check for user access or permission in Drupal 8"
date: 2014-10-30 00:50:17 -0500
comments: true
categories:
---
In Drupal 7, you would use the user_access function to check for user access. Here's how to do it in Drupal 8.

``` php How to check for permission in Drupal 8
// Get the current user
$user = \Drupal::currentUser();

// Check for permission
$user->hasPermission('access administration menu');
```