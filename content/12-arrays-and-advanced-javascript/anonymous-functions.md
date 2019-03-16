+++
date = "2017-01-22T18:04:24-05:00"
title = "Anonymous Functions"
toc = true
next = "/12-arrays-and-advanced-javascript/looping-through-arrays"
prev = "/12-arrays-and-advanced-javascript/array-overview"
weight = 8

+++

## What are Anonymous Functions?

```js

// An anonymous function is a function without a name

function(width, height){
  return width * height;
};


// this function can later be stored as a variable and used later in your code

var area = function(width, height){
  return width * height;
};

// Call anonymous function stored as a variable

area(4, 5); // returns 20

```
---

## When should you use Anonymous Functions?

- Use for code that only needs to run once within a task

- Use as an event handlers to perform a task when an event occurs

{{% notice tip %}}
  Event handlers are functions that are called when an event is triggered
{{% /notice %}}

---

## Using an anonymous function as an event handler

```js

// Uses a *named function* to serve as a event handler (function that is called as a result of an event)

$('#blueButton').click(blueEffect);

function blueEffect(){
  $('body').css('background-color', 'blue');
};

```

```js


// Results are same as above example, but instead we use an anonymous function as a click handler
// This is the common jQuery pattern

$('#blueButton').click(function(){
  $('body').css('background-color', 'blue');
});

```
