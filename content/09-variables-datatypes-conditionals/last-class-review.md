+++
date = "2017-01-22T18:04:24-05:00"
title = "Last Class Review"
toc = true
next = "/09-variables-datatypes-conditionals/code-along-1"
prev = "/09-variables-datatypes-conditionals/agenda"
weight = 6

+++

## DOM

- Document Object Model

- Browsers views HTML pages as documents and provides developers with a means of programatically referencing HTML pages using Javascript

---

## What is jQuery?

- A Javascript library that allows developers to **manipulate the DOM** using CSS selectors

- jQuery provides an alternative (more intuitive) way of referencing the DOM (HTML elements) so we can add behavior to our pages


```js

  // selecting an element using native/pure javascript
  document.getElementById('flavors');

```

vs

```js

  // using jQuery (same as above but with much more intuitive syntax)
  $('#flavors');

```

{{% notice tip %}}
  Anything that can be done in jQuery can be done with native Javascript, just with less code
{{% /notice %}}

---

## What jQuery Isn't

- jQuery isn't another programming language (it's Javascript)




