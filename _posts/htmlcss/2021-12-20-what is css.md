---
layout: single
title: "What is CSS?"
date: 2021-12-20 18:00:00 +0100
categories: htmlcss
tags: css
---

**Notice!** _*These posts are basically my learning notes.*_  
There can misinformation and mistakes :(  
If you find any wrong info, please leave a comment and I will get to it asap!  
{: .notice--warning}

# How to add CSS to HTML Page

- Now that we have the bone, HTML, written down, we need add the muscle and skin, CSS.
- There are two ways of doing this
- Add CSS directly on the HTML file (Not Recommended)
- Make separate CSS file and link it to the HTML file

## Inline CSS

- This is not really a recommended option but if needed, you can add `<style> </style>` tag in the `<head>`
- In this `<style>` tag, you can input the CSS code you want to apply to your HTML file

## Making a separate CSS file

- First, you should make a link for your CSS file on the HTML `<head>`
- Typically, the main CSS file is named “styles.css”
- Thus you will make your `<link />` tag as below

```html
<link href="styles.css" rel="stylesheet" />
```

- Now you can create your “styles.css” in the directory and write CSS code in the file

# How does CSS work

## How to write CSS code

- CSS code works like this
- All CSS codes will have a selector
- Selector is the HTML element that the CSS code is pointing to
- It can be a tag, class or ID(there are also pseudo selectors)
- After choosing the selector, you put a set of curly bracket -> { }
- Within this, you write the properties you want the selector to have

```css
h1 {
  color: blue;
  font-size: 24px;
}
```

- selector { property-name: property-value
  }

## Cascading Style Sheets

- CSS is actually abbreviation for Cascading Style Sheets
- Cascading means it’s falling down like a waterfall or something like a stair structure
- This means that the browser is reading the CSS code from top to bottom
- If you write two lines that both have h1 as selector, have same property but different property-value, only the later one will be applied
- This means that the order of your CSS code matters
