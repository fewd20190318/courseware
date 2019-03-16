+++
date = "2017-01-22T18:04:24-05:00"
title = "Returning Values from Functions"
toc = true
prev = "/10-functions/calling-functions"
next = "/10-functions/working-with-parameters"
weight = 11

+++


- Many times you will write a function and expect a value to be returned - this is called a **return value**

- to have your function return a value you must use the `return` keyword in the last line of the body of your function

- You can store the returned value in a variable and use it for later

```js

// declare a function called bark
// that *returns* a string respreseting 'woof woof'
function bark() {
  return 'woof woof!';
}

// call the bark function and store result in a variable
var sound = bark();

// print out result to the console
console.log('a dog makes the following sound ' + sound);

```

<a class="jsbin-embed" href="https://jsbin.com/parizup/embed?js,console">JS Bin on jsbin.com</a><script src="https://static.jsbin.com/js/embed.min.js?3.41.0"></script>



- If you don't use the `return` keyword, then no value will be returned

```
// declare a function called meow
// that generates a string representing 'meow' but 
// does not use the return keyword

function meow() {
  'meow';
}  

// call the meow function and store result in a variable
var sound = meow();

// print out result to the console
console.log('a cat makes the following sound ' + sound);


```

<a class="jsbin-embed" href="https://jsbin.com/vagacoy/embed?js,console">JS Bin on jsbin.com</a><script src="https://static.jsbin.com/js/embed.min.js?3.41.0"></script>
