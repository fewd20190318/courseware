+++
date = "2017-01-22T18:04:24-05:00"
title = "$() function"
toc = true
prev = "/08-intro-to-jquery/adding-jquery"
next = "/08-intro-to-jquery/document-ready"
weight = 12

+++

- jQuery uses a function called jQuery() to find elements on the page

- $() is shorthand for jQuery(); $() is what is used most often

```javascript

// both of these creates a jQuery object around
// the <p> element(s)
// This allows you to use jQuery methods on the element

jQuery('p') === $('p');

```

{{% notice tip %}}
We'll be using the **$(selector)** syntax exclusively in this class
{{% /notice %}}
