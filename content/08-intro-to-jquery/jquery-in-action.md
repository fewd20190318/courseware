+++
date = "2017-01-22T18:04:24-05:00"
title = "jQuery in Action"
toc = true
prev = "/08-intro-to-jquery/document-ready"
next = "/08-intro-to-jquery/code-along"
weight = 14

+++

- Here are some examples of things you can do with jQuery

- This is not a exhaustive list (not possible)


---

## Select Elements using CSS Selectors

<a class="jsbin-embed" href="https://jsbin.com/kihima/embed?js,output">JS Bin on jsbin.com</a><script src="https://static.jsbin.com/js/embed.min.js?3.41.0"></script>



---
## Getting and Setting Content using jQuery

Using methods like `.html()`, `.text()`  and `.val()` you can **get** (i.e. retrieve) and **set** content on your pages

```javascript
  // get the text content stored in an element
  $('p.intro').text();

  // set the content to another value
  $('p.intro').text('Updated text that will replace existing content');

```

<a class="jsbin-embed" href="https://jsbin.com/faxule/embed?html,css,js,output">JS Bin on jsbin.com</a><script src="https://static.jsbin.com/js/embed.min.js?3.41.0"></script>


<a class="jsbin-embed" href="https://jsbin.com/zevoko/embed?js,output">JS Bin on jsbin.com</a><script src="https://static.jsbin.com/js/embed.min.js?3.41.0"></script>

---

## Adding New Content using jQuery .prepend() / .append()

Using methods like `.prepend()` and `.append()` you can dynamically add elements to html to your pages

<a class="jsbin-embed" href="https://jsbin.com/qamikaw/embed?js,output">JS Bin on jsbin.com</a><script src="https://static.jsbin.com/js/embed.min.js?3.41.0"></script>

---

## More Examples

- See examples in **js_examples** (in the starter_code) folder for more examples


