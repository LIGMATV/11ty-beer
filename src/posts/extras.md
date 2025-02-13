---
title: Extras
description: Some extra features like Image and Icon shortcodes.
date: 2025-02-13
tags:
 - tutorial
snippet:
    image: "{% image '/img/480x400.webp' 'Not so big' '480x400' 'lazy' %}"
    icon: "{% icon 'mdi:home-city-outline' %} Some text {% icon 'si:lastdotfm' %}"
---

## Images

You can use image shortcode to adjust image sizes and loading specifier. [(Utilities source)](https://github.com/LIGMATV/11ty-beer/blob/main/_utilities/imageShortcode.js)

Example:  
```nunjucks
{{ snippet.image }}
```
Code result:
```html
{% image '/img/480x400.webp' 'Not so big' '480x400' 'lazy' %}
```
Preview:  
{% image '/img/480x400.webp' 'Not so big' '480x400' 'lazy' %}

## Icons

11ty Beer uses [eleventy-plugin-icons](https://github.com/uncenter/eleventy-plugin-icons) to use icon shortcodes, [Simple Icons](https://simpleicons.org/) and [Pictogrammers MDI](https://pictogrammers.com/library/mdi/) are supported. [(Utilities source)](https://github.com/LIGMATV/11ty-beer/blob/main/_utilities/getIcons.js)  
In this example, [`home-city-outline`](https://pictogrammers.com/library/mdi/icon/home-city-outline/) from [Pictogrammers MDI](https://pictogrammers.com/library/mdi/) and [`lastdotfm`](https://simpleicons.org/?modal=icon&q=lastdotfm) from [Simple Icons](https://simpleicons.org/) are used.

Example:
```nunjucks
{{ snippet.icon }}
```
Code result:
```html
{% icon 'mdi:home-city-outline' %} Some text {% icon 'si:lastdotfm' %}
```
Preview:
{% icon 'mdi:home-city-outline' %} Some text {% icon 'si:lastdotfm' %}