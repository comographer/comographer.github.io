---
layout: single
title: "CSS Theory - Position"
date: 2021-12-24 12:00:00 +0100
categories: htmlcss
tags: css position
---

**Notice!** _*These posts are basically my learning notes.*_  
There can misinformation and mistakes :(  
If you find any wrong info, please leave a comment and I will get to it asap!  
{: .notice--warning}

# What is Position Property

- The position CSS property sets how an element is positioned in a document
- Depending on the property value, they can be `static`, `relative`, `absolute`, `fixed` or `sticky`

## Fixed Position

- if an element is `position: fixed;`, whether you scroll or change screen size, the element will stay in that position
- If you give `top`, `right`, `bottom` or `left` property to an element that is `position: fixed;`,
  this will determine the fixed location of that element and will ignore other elements
- Usually you can use this for the menu bar on the top part of a website

## Static Position

- This is the default position
- `position: static;` will just place the element where you placed them initially

## Relative Position

- When you use `position: relative;`, you can use `top`, `right`, `bottom` or `left` to move around the element relative to its position while it was static
- The starting position is based on the parent element

## Absolute Position

- This one is more similar to Position Relative but more extreme
- By using `position: absolute;`, the element will move based on the the closest **relative parent element** and not the direct parent element unless direct parent is position relative
- if HTML is written as below:

```html
<body>
  <div class="”directParent”">
    <div class="”absolute”"></div>
  </div>
</body>
```

- And CSS as below:

```css
.absolute {
  position: absolute;
  right: 0px;
}
```

- `.absolute` will position based on `<body>`, instead of `.directParent` because `<body>` is the closest **relative parent element**
