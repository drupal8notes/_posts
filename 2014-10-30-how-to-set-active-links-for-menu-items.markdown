---
layout: post
title: "How to set active links for menu items"
date: 2014-10-30 00:37:39 -0500
comments: true
categories: 
---

In your THEMENAME.theme file, add the following code:

``` php Implements hook_preprocess_menu()
/**
 * Implements hook_preprocess_menu().
 */
function THEMENAME_preprocess_menu(&$variables, $hook) {
  if ($hook == 'menu__main') { // We're doing that for main menu.
    // Get the current path.
    $current_path = \Drupal::request()->getRequestUri();
    $items = $variables['items'];
    foreach ($items as $key => $item) {
      // If path is current_path, set active to li.
      if ($item['url']->toString() == $current_path) {
        // Add active link.
        $variables['items'][$key]['attributes']['class'] = 'active';
      }
    }
  }
}
```
