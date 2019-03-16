+++
date = "2017-01-22T18:04:24-05:00"
title = "Looping through Arrays"
toc = true
next = "/12-arrays-and-advanced-javascript/code-along"
prev = "/12-arrays-and-advanced-javascript/anonymous-functions"
weight = 8

+++

## Loops and Interation

- Loops offer a quick and easy way to do something repeatedly

- 

{{% notice tip %}}
Javascript offers many different ways to loop, [click here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Loops_and_iteration) for more information
{{% /notice %}}

---

## Using .forEach() (native javascript)

- Native javascript offers a .forEach() method loops through (iterates) an array

```js
  var fruits=[“Banana”,”Apple”,”Pear”];

  fruits.forEach(function(element,index){
    console.log(element,index);
  });

```

<a class="jsbin-embed" href="https://jsbin.com/kurivux/embed?js,output">JS Bin on jsbin.com</a><script src="https://static.jsbin.com/js/embed.min.js?3.41.3"></script>

{{% notice tip %}}
[click here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/forEach) for more information about the forEach() loop
{{% /notice %}}


---

## Using $.each() (jQuery)

- jQuery also provides a way to iterate arrays through its $.each() method

```js
  var fruits=[“Banana”,”Apple”,”Pear”];

  $.each(fruits, function(index, element){
    console.log(index, element);
  });

```

<a class="jsbin-embed" href="https://jsbin.com/polewov/embed?js,output">JS Bin on jsbin.com</a><script src="https://static.jsbin.com/js/embed.min.js?3.41.3"></script>

{{% notice tip %}}
[click here](https://api.jquery.com/each/) for more information about the jQuery's $.each() loop
{{% /notice %}}

