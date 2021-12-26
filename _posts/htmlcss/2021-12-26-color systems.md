---
layout: single
title: "CSS Theory - Color Systems(Hexadecimal, RGBA)"
date: 2021-12-26 12:00:00 +0100
categories: htmlcss
tags: css
---

**Notice!** _*These posts are basically my learning notes.*_  
There can misinformation and mistakes :(  
If you find any wrong info, please leave a comment and I will get to it asap!  
{: .notice--warning}

![Color](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/546b520f-cd4b-4511-a0ed-7486f6f4aa27/color_systems.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20211226%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20211226T182228Z&X-Amz-Expires=86400&X-Amz-Signature=e211551713ff3b1aee542f23304eb4d893a32dd3d6d533301d74d3f7ca1b81d2&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22color%2520systems.png%22&x-id=GetObject)

# Hexadecimal system

- Hexadecimal system is a coloring system that has 6 digits followed by `#` to represent a color
  `#3da56e`

# RGBA

- RGBA uses Red, Green and Blue from 0 to 255 to represent color
- You can also add opacity to RGBA color
  `rgb(61, 165, 110)` This is without opacity
  `rgba(61, 165, 110, 0.5)` This is with 50% opacity

# How to utilize colors as variable

- If you are using same color in many different elements, you can save the color as variable in CSS

```css
:root {
  —main-color: #3da56e;
}
div {
  background-color: var(—main-color);
}
span {
  color: var(—main-color);
}
```

- Other things can be saved in the `:root` as variable and this will save a lot of time
