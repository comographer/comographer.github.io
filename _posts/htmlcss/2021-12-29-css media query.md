---
layout: single
title: "CSS Theory - Media Query"
date: 2021-12-29 12:00:00 +0100
categories: htmlcss
tags: css mediaquery
---

**Notice!** _*These posts are basically my learning notes.*_  
There can misinformation and mistakes :(  
If you find any wrong info, please leave a comment and I will get to it asap!  
{: .notice--warning}

# Media Queries

## Setting up Media Query

- Using Media Query, you can detect the screen size of the user
- And depending on that, you can show different CSS

```html
<body>
  <div></div>
</body>
```

```css
div {
  width: 200px;
  height: 200px;
  background-color: teal;
}
@media screen and (max-width: 600px) {
  div {
    background-color: tomato;
  }
}
```

- Above code will show the user a box with color teal when screen width is larger than 600px
- But as soon as the screen width is smaller than 600px, box color will change to tomato

## More Conditions

- other than `min-width` and `max-width`, you can also add more conditions
- `orientation: landscape` and `orientation: portrait` detects which orientation the viewer's phone is in
- [MDN](<[https://developer.mozilla.org/en-US/docs/Web/CSS/Media_Queries/Using_media_queries](https://developer.mozilla.org/en-US/docs/Web/CSS/Media_Queries/Using_media_queries)>)
