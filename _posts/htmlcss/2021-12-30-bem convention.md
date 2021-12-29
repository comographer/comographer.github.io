---
layout: single
title: "BEM Naming Convention"
date: 2021-12-30 12:00:00 +0100
categories: htmlcss
tags: bem
---

**Notice!** _*These posts are basically my learning notes.*_  
There can misinformation and mistakes :(  
If you find any wrong info, please leave a comment and I will get to it asap!  
{: .notice--warning}

> Not only for HTML & CSS, but for any kind of coding, naming your components is probably the hardest thing to do  
> In order to make this easier to do and also to easily work with other people, there are conventions that are widely accepted

# BEM

## Block Element Modifier

- Among many conventions, BEM is probably the most widely used convention when it comes to naming classes in HTML & CSS
- It divides the user interface into several blocks thus making it easy to keep track of your code

### Block

- Blocks are standalone entitiy that is meaningful on its own
- examples
- `header`, `list`, `menu`, etc

### Element

- Elements are part of a block that can't exist alone and are semantically tied to a block
- examples
- `header` `title`, `list item`, `menu item`, etc

### Modifier

- A flag on a block or an element to modify appearance or behavior
- examples
- `disabled`, `fixed`, `color yellow`, etc

## Naming Rules

### Block

- Block names may consist of Latin letters, digits, and dashes
- HTML

```html
<div class="block">...</div>
```

- CSS
  ```css
  .block {
    color: tomato;
  }
  ```

### Element

- Element names may consist of Latin letters, digits, dashes and underscores
- CSS class is formed as block name plus two underscores plus element name: `.block__elem`
- HTML

```html
<div class="block">
  ...
  <span class="block__elem"></span>
</div>
```

- CSS
  ```css
  .block\_\_elem {
    color: teal;
  }
  ```

### Modifier

- Modifier names may consist of Latin letters, digits, dashes and underscores
- CSS class is formed as block's or element's name plus two dashes: `.block--mod` or `.block__elem--mod` and `.block--color-black` with `.block--color-red`
- Spaces in complicated modifiers are replaced by dash
- HTML

```html
<div class="block block—mod">
  ...
  <div>
    <div class="block block—size-big block—shadow-yes">...</div>
  </div>
</div>
```

- CSS

```css
.block—mod {
}

.block—mod .block__elem {
}
```
