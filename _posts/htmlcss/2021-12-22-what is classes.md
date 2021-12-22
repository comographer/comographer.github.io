---
layout: single
title: "CSS Theory - Classes"
date: 2021-12-22 18:00:00 +0100
categories: htmlcss
tags: css
---

**Notice!** _*These posts are basically my learning notes.*_  
There can misinformation and mistakes :(  
If you find any wrong info, please leave a comment and I will get to it asap!  
{: .notice--warning}

# Classes

## Types of selectors

- There are many ways of selecting HTML element from CSS
- You can use the tag or id as selector
- Using tag as selector is used often in bigger picture
- But when getting into details, you sometimes need to select a single or just a few element out of the same tag
- Id can be used for this but since ids are to be unique value, you can’t use the same id for multiple element
- To solve this, in most cases, you will be using classes

## What is Class

- Class can be used in many places in repetition
  ```html
  <span class="sample"> Hello World </span>
  ```
- When selecting a class in CSS, you can select by adding a dot in front of the class name
  ```css
  .sample {
    background-color: tomato;
  }
  ```
- HTML Elements can have multiple classes by having spaces between class names
  ```html
  <div class="class1 class2 class3">Many classes</div>
  ```
- By utilizing tag selector and class selector, you can code CSS efficiently
