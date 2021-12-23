---
layout: single
title: "CSS Theory - Flexbox"
date: 2021-12-23 12:00:00 +0100
categories: htmlcss
tags: css flexbox
---

**Notice!** _*These posts are basically my learning notes.*_  
There can misinformation and mistakes :(  
If you find any wrong info, please leave a comment and I will get to it asap!  
{: .notice--warning}

> Since inlines and blocks have their limitation, something better was invented
> A way to move around and position boxes more flexibly : Flexbox

# Flexbox

- It will be explained in the Rules, but you should apply the property  
  `display: flex;`  
   to the parent element of the element you want to apply flexbox to
- When you apply flexbox, there are many properties that are now available

## Rules of Flexbox

- You do not talk to the children, you talk to the parent element

- If there is HTML code like below :

```html
<main>
  <div></div>
  <div></div>
  <div></div>
</main>
```

- In order to apply flexbox to <div>s, you apply flexbox property to <main>

```css
main {
  display: flex;
}
```

- `justify-content` align items according to the main axis of the flexbox
- `align-items` : align items according to the cross axis of the flexbox

![main and cross axis](https://cms-assets.tutsplus.com/cdn-cgi/image/width=1700/uploads/users/30/posts/30183/image/axes.png)

# Flexbox Properties

## Direction

- The main axis and cross axis can be inverted using `flex-direction`
- the property value default of `flex-direction` is `row`
- By changing this value between `row` `row-reverse` `column` `column-reverse`, you can invert and flip the main axis and cross axis

## Wrap

- By using the property `flex-wrap` and correct values, you can make flex children to wrap around depending on screen size
- If you do `flex-wrap: wrap;`, elements will wrap around if there isn’t enough space to fit in

# Practice Flexbox

[https://flexboxfroggy.com/](https://flexboxfroggy.com/)
