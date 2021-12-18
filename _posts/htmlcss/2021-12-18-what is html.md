---
layout: single
title: "What is HTML?"
date: 2021-12-18 18:00:00 +0100
categories: htmlcss
tags: html
---

**Notice!** _*These posts are basically my learning notes.*_  
There can misinformation and mistakes :(  
If you find any wrong info, please leave a comment and I will get to it asap!  
{: .notice--warning}

# Basic Info

- HTML is the markup language that describes the content of a website
- HTML doesn’t have error - Browser will try to show you content even if HTML is wrong
- You put your content between and opening tag and its corresponding closing tag

```html
<h1>Hello this is a title</h1>
```

- Some tags like anchor tag `<a>` can be more complex thus requiring more info which are called attributes.  
  For example, `<a>` requires an `href` or hyperlink reference attribute like this.
  ```html
  <a href=“https://google.com”>Go to google.com</a>
  ```
- Some tags don’t require closing tag because they are a self-closing tag `<img />`  
  These self-closing tags don’t require any text thus don’t need to have opening and closing tag.  
  Just like an image which is the content itself.

# Structure of HTML document

## The Structure

- First line is always `<!DOCTYPE html>`  
  this makes it easier for the browser to know this is an HTML document

- `<html> </html>` comes after
- `<head> </head>` is between
- `<body> </body>` is after head
- The basic structure looks something like this

```html
<!DOCTYPE html>
<html>
  <head> </head>
  <body></body>
</html>
```

## HEAD

- Head is where we configure the website.
- Things such as `<title> </title>`, `<link />`, `<meta />`, etc. will go here
- When you are linking CSS and Javascript to HTML, they also come here
- In most cases, the content of the tags in Head will be invisible on the page itself
- Most information here are to be read by browsers and search engines

## Tags Tags

- In Head and Body, we will need to use a lot of tags
- There is no way we can memorise all the tags
- When in doubt, best place to look is [MDN](https://developer.mozilla.org/)
- You can find any Tag or Attributes you need for HTML, CSS and Javascript
- ```html
  <tagname attrname="“attrvalue”">Content</tagname>
  ```

## Semantic HTML

- Some tags can mean something to the programmer but can’t be seen intuitively to the user
- `<main>` or `<header>` are some of the most well known of these types
- These are basically boxes that contain other tags and helps in making structure of the website
- By using semantic tags, we can make websites more understandable programming wise and thus makes development easier
