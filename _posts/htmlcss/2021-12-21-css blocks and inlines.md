---
layout: single
title: "CSS Theory - Blocks and Inlines"
date: 2021-12-21 18:00:00 +0100
categories: htmlcss
tags: css
---

**Notice!** _*These posts are basically my learning notes.*_  
There can misinformation and mistakes :(  
If you find any wrong info, please leave a comment and I will get to it asap!  
{: .notice--warning}

# Blocks and Inlines

- Blocks do not let anything come next to it
- Most used block is `<div>`
- Inlines allow other elements to come next to it
- Most used inline is `<span>`
- Understanding these concepts help when design a website
- Usually except for `<span>`, `<a>` and `<image>`, most elements are blocks

# Changing between Block and Inline

- It is actually possible to change between block and inline
- In CSS, you can use the `display` property to change between block and inline
- However, when changing block into inline, you need to know that **inlines don’t have height and width**

## Three features of blocks

- **Margin**, **Padding**, **Border** are the main features of a block

![margin-border-padding](/assets/images/block_features.png)

### Margin

- Margin is the area from the border of the box to the outside
- When applying margin to an element, you can apply on four sides, `margin-top`, `margin-left`, `margin-right`, `margin-bottom`
- But no one wants to write four lines of code for margin
- Shortcut is as below

```css
div {
  margin: 10px; /* giving margin of 10px to all sides */
  margin: 10px 20px; /* giving top and bottom 10px and left and right 20px margin */
  margin: 5px 10px 15px 20px; /* top 5px, right 10px, bottom 15px, left 20px */
}
```

- Collapsing Margin : When two blocks that are aligned have borders touching each other,  
  their margins become one - Not entirely sure about this concept

### Padding

- Padding is the space from border of the box to the inside

### Border

- Border is bascially the border of the box
- There are many types of borders but in most cases, you will only be using `border-style: none or solid`

## Inline

- Something to note about inlines is that as mentioned, they don’t have width and height
- Also, they can have padding on all sides but cannot have margin top and bottom

### Inline-Block

- In order to overcome the above mentioned properties of inlines, we can change elements into inline-blocks which can have elements next to them like inline but at the same time have width, height and margin top and bottom
  `div {display: inline-block;}`
- This may seem like it’s the ultimate solution but inline-blocks actually have many issues
- It has some weird default values and it messes with the layout
- More importantly, inline-block doesn’t support responsive design
