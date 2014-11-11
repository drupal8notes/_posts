---
layout: post
title: "drupal_get_form in Drupal 8"
date: 2014-11-11 12:16:57 -0500
comments: true
categories: 
---
In Drupal 8 you use the FormBuilder service to retrieve forms.

```
$form = \Drupal::formBuilder()->getForm('Drupal\search\Form\SearchBlockForm');
```

The argument passed to the getForm() method is the name of the class that defines your form and is an implementation of \Drupal\Core\Form\FormBuilderInterface. If you need to pass any additional parameters to the form, pass them on after the class name.

```
$form = \Drupal::formBuilder()->getForm('Drupal\search\Form\SearchBlockForm', $foo);
```