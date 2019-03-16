+++
date = "2017-01-22T18:04:24-05:00"
title = "$(this)"
toc = true
next = "/12-arrays-and-advanced-javascript/lab"
prev = "/12-arrays-and-advanced-javascript/code-along"
weight = 11

+++

## $(this)

- ``this`` one of the most misunderstood concepts in javascript
- ``this`` (pure javascript) refers to the owner of a function
- ``$(this)`` (jquery) gives you reference to uses jQuery to select the current element

---

## Example of $(this) in use

```js

// Event that makes the <p> element disappear when it is clicked

$('p').click(function(){

  // $(this) refers to the jQuery element, $(p), that
  // the click event was called on

  // Tell the <p> element to hide itself
  $(this).hide();
});

```

<a class="jsbin-embed" href="https://jsbin.com/fideyac/embed?html,css,js,output">JS Bin on jsbin.com</a><script src="https://static.jsbin.com/js/embed.min.js?3.41.3"></script>


---

## Active Link Example using $(this)

- The following is example of how a developer could go using javascript to implement an "active link" effect

<a class="jsbin-embed" href="https://jsbin.com/tipilod/embed?js,output">JS Bin on jsbin.com</a><script src="https://static.jsbin.com/js/embed.min.js?3.41.3"></script>
