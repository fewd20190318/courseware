+++
date = "2017-01-22T18:04:24-05:00"
title = "Breakpoints"
toc = true
next = "/14-responsive-design/progressive-enhancement"
prev = "/14-responsive-design/media-query-parts"
weight = 14

+++

## What are Breakpoints?

- The points where your css style will change as a result of your media queries

```


  @media only screen and (min-width: 320px) {
    /* Styles */
  }

  @media only screen and (min-width: 320px) and (orientation: landscape) {
    /* Styles */
  }

  @media only screen and (min-width: 321px) and (max-width : 700px) {
    /* Styles */
  }

  @media only screen and (min-width: 701px) {
    /* Styles */
  }

```

---

## Recommended "Starting" Breakpoints

- 320px
- 480px
- 600px
- 768px
- 900px
- 1200px

{{% notice tip %}}
Breakpoints should be selected based on your specific design
{{% /notice %}}
