+++
date = "2017-01-22T18:04:24-05:00"
title = "Adding jQuery to your projects"
toc = true
prev = "/08-intro-to-jquery/jquery-intro"
next = "/08-intro-to-jquery/dollar-sign-function"
weight = 11

+++

## There are two ways to add jQuery to your projects

 - download a jQuery file and store it within your project

 - Use a CDN (content delivery network)

---

### Option #1 - Download jQuery file(s)

```html
<html>
  <head>
    <title>Add jQuery by downloading jQuery file(s)</title>
  </head>
  <body>

    <script src="js/jquery-2.1.4.js"></script>
    <script src="js/app.js"></script>
  </body>
</html>

```
---

### Option #2 - Use a CDN (Content delivery network)

```html
<html>
  <head>
    <title>Add jQuery using a CDN</title>
  </head>
  <body>

    <script src="//code.jquery.com/jquery-2.1.4.js"></script>
    <script src="js/app.js"></script>
  </body>
</html>

```
---

## Content Delivery Networks (CDNs)

- A content delivery network (CDN) places files in different locations so that the person using your webpage can receive the nearest 
copy of it faster

- Prevents your users' browsers from downloading commonly used libraries(like jQuery) every time they visit your site

- Use of CDNs increases page speed for highly trafficked sites

- Click [here](https://varvy.com/pagespeed/content-delivery-networks.html) for a nice overview of CDNs
