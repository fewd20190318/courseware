+++
date = "2017-01-22T18:04:24-05:00"
title = "Viewport Meta Tag"
toc = true
next = "/14-responsive-design/media-query-overview"
prev = "/14-responsive-design/mobile-websites"
weight = 11

+++

## What is the viewport?

- Area on the computer or device screen where you are viewing a web page

- Viewport width is not always the same thing as screen width

 - For example: A person's labtop may have a maximum **screen width** of 1280px, but likes to resize their web browser to 800px (**viewport width**)

- On **mobile devices viewport width is the same as screen width** because mobile devices don't allow you to change the size of your browser

---

## Viewport Meta Tag

Add the following to your <head> element

-  This enables use of media queries for cross-device layouts.

```html

<meta name="viewport" content="width=device-width, initial-scale=1">

```

[More info on the viewport meta tag](http://webdesign.tutsplus.com/articles/quick-tip-dont-forget-the-viewport-meta-tag--webdesign-5972)

---

## What happens if you don't set the viewport?

![inline](/images/14/non_responsive_site_on_phone.png)


- For example, the default width for iPhones is 980 pixels 
the browser is rendering the page as if the browser window was 980 pixels wide, but then shrinking it down to ⅓ of the size so that it fits on a screen that’s only 320 pixels wide

---

## Width

- Tells the browser how to scale the web page

- For a responsive site, the value width=device-width tells the browser to render the page at full size, whatever the size may be

- The browser is rendering the page so that the viewport width is the actual width of the device (i.e., at 100%)


---

## Initial-Scale

- Tells the browser how to scale the web page when it’s first loaded on the screen (i.e., the zoom factor)

- initial-scale=1 means that the page will be rendered at the size determined by the width attribute, and will not be zoomed in or out

- If you use a number larger than 1, then the page will be zoomed to that level

 - For example, an initial-scale=2 value would mean that the page would be zoomed to be twice as large as actual size, so you would only see half of the page on the screen

- initial-scale value only determines the size of the web page when it’s first loaded on the screen. Remember that your mobile device also gives users the ability to zoom in and out
