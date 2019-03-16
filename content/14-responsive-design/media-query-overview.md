+++
date = "2017-01-22T18:04:24-05:00"
title = "Media Query Overview"
toc = true
next = "/14-responsive-design/media-query-parts"
prev = "/14-responsive-design/mobile-websites"
weight = 12

+++

## What are the Media Queries?

- Key element in responsive design

- Allow you to apply different styles based on the screen size of the user's device (viewport)

- Media Queries ask questions - Is the width of the viewport greater than 240px?

- Media queries don’t affect the HTML (the actual content and structure of the underlying page) — they only affect the styles that are applied to the page using CSS


^
- Browsers starting supporting media queries in 2009
- The media queries that are common in responsive design is the width of a device’s viewport, not the screen. The viewport
is the area on the screen (inside the browser window) in which a website is displayed.

---

## Media Query Example

```

body {
  background-color: green;
}

@media only screen and (min-width: 480px){
  body {
    background-color: blue;
  }
}

```

This query is asking "If this is a screen and the viewport greater than or equal to 480 pixels?" If so, make the background color blue.

