---
layout: single
title: "CSS Theory - Transitions"
date: 2021-12-27 12:00:00 +0100
categories: htmlcss
tags: css
---

**Notice!** _*These posts are basically my learning notes.*_  
There can misinformation and mistakes :(  
If you find any wrong info, please leave a comment and I will get to it asap!  
{: .notice--warning}

# Transition

## What is Transition

- When you have different CSS for default state and different states such as `hover`,
  you can add transition effect to create animation
- This `transition` property should go on the **default state**
- The property value should be

1. The changing property
2. Duration
3. Timing function

- You can add to multiple properties by adding `,`

```css
div {
  color: white;
  background-color: tomato;
  transition: background-color 5s ease-in-out, color 5s ease-in-out;
}

div:hover {
  color: black;
  background-color: teal;
}
```

- Of course if `Duration` and `Timing function` are the same, you can replace property with `all`

```css
div {
  color: white;
  background-color: tomato;
  transition: all 1s ease-in-out;
}
```

## Timing Function

- There are many different `Timing Function` which determines the timing of the transition
- Default functions are `ease`, `linear`, `ease-in`, `ease-out` and `ease-in-out`
- You can check the default and many other functions [here](<[https://matthewlein.com/tools/ceaser](https://matthewlein.com/tools/ceaser)>)
- You can customize the effect timing with `cubic-beizer`

## Transformation

- Transition is also powerful when combined with Transformation
- Check out transformation on [MDN](<[https://developer.mozilla.org/ko/docs/Web/CSS/transform](https://developer.mozilla.org/ko/docs/Web/CSS/transform)>)
