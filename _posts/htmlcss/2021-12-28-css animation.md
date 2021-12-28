---
layout: single
title: "CSS Theory - Animation"
date: 2021-12-28 12:00:00 +0100
categories: htmlcss
tags: css animation
---

**Notice!** _*These posts are basically my learning notes.*_  
There can misinformation and mistakes :(  
If you find any wrong info, please leave a comment and I will get to it asap!  
{: .notice--warning}

# Animation

## How to Create CSS Animation

- In order to create CSS Animation, you need to create keyframes
- You can place it at the top of the CSS file as below

```css
@keyframes animationName {
}
```

- Inside, you need to set `from` and `to`

```css
@keyframes animationName {
  from {
    transform: rotateX(0);
  }
  to {
    transform: rotateX(360deg);
  }
}
```

- After animation is setup on keyframe, you can input the the animation to an element as below

```css
div {
  animation: animationName 3s ease-in-out inifinite;
}
```

- Adding `infinite` will play the animation over and over

## Making Smooth Animation

- In order to make animation more smooth, instead of setting `from` and `to`, you can replace them with percentages

```css
@keyframes animationName {
  0% {
    transform: rotateX(0);
  }
  50% {
    transform: rotateX(180deg) translateY(-100px);
  }
  100% {
    transform: rotateX(0);
  }
}
```

- When you make 0% and 100% same, animation will finish at the same position thus making the repitition more smooth
