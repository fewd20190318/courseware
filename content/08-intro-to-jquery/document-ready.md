+++
date = "2017-01-22T18:04:24-05:00"
title = "Document Ready Function"
toc = true
prev = "/08-intro-to-jquery/dollar-sign-function"
next = "/08-intro-to-jquery/jquery-in-action"
weight = 13

+++


- jQuery must wait for a page to be loaded before it can manipulate the page's DOM

- jQuery provides a "document ready" function that will run once the DOM is fully loaded

- There are two ways to express the "document ready" function for jQuery

---

### Option #1: Long form syntax

```javascript
$(document).ready(function(){
  // place your code here
  // jquery code must be placed inside of a document ready block
})

```

---


### Option #2: Short form alternative syntax

```javascript
$(function(){
  // this is the same as the $(document).ready(function(){}) function
  // just much less code

  // place your code here
});

```


{{% notice tip %}}
	There are no advantages to choosing one syntax over the other. However, option #2 is less typing :)
{{% /notice %}}
