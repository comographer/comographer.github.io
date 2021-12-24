---
layout: single
title: "CSS Theory - Pseudo Selector"
date: 2021-12-25 12:00:00 +0100
categories: htmlcss
tags: css pseudoselector
---

**Notice!** _*These posts are basically my learning notes.*_  
There can misinformation and mistakes :(  
If you find any wrong info, please leave a comment and I will get to it asap!  
{: .notice--warning}

# Pseudo Selector

## Non Pseudo Selectors

- So far, we know three ways of selecting HTML element from CSS
- The name of the **tag**: by simply writing the name

```css
div {
  width: 100px;
}
```

- The name of the **id** combined with `#`

```css
#sampleId {
  height: 100px;
}
```

- The name of the **class** combined with `.`

```css
.sampleClass {
  position: absolute;
}
```

## What is Pseudo Selector

- Above method is great and should be used in most cases
- However, sometimes you might want to select, for example, the last `div` or the first one
- These kind of complex selections can be achieved using pseudo selector
- Pseudo Selector can be used by adding `:` after regular selector and choosing the pseudo selector

```css
div:last-child {
  background-color: whitesmoke;
}
```

- Above CSS will apply background-color of whitesmoke only on the div that is the last-child
- you can choose not only first or last child but there are many options like `span:nth-child(even)` which will apply only to the even number spans

## Combinators

- It is also possible to combine selectors depending on parent-child relation of the selectors
- If you want to change the color of `span`s only when they are inside `p`, try the below

```css
p span {
  color: tomato;
}
```

- This will only color the `span`s that are inside `p`
- You can also add more parents as long as it follows the structure of the HTML
- If you want to. apply the above only to the direct children, you can add `>` between `p` and `span`

```css
p > span {
  color: tomato;
}
```

- If you want to apply above to the `span` that is next to(brother) of `p`, you can add `+` between `span` and `p`

```css
p + span {
  color: tomato;
}
```

- If you have something between `p` and `span` but still want to keep above property, you can use `~` instead of `+`

## State

- Selectors can also point out to the state of HTML elements
- Most useful are `active`, `hover`, `focus`, `visited` and `focus-within`

## Practicing Pseudo Selectors

- There are much more to Pseudo Selector
- You can also choose according attributes of HTML and much more
- One of the best place to practice is the link below
- [Pseudo Selector Practice](<[https://flukeout.github.io/](https://flukeout.github.io/)>)
