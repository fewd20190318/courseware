+++
date = "2017-01-22T18:04:24-05:00"
title = "Functions Calling Other Functions"
toc = true
prev = "/10-functions/working-with-parameters"
next = "/10-functions/code-along-1"
weight = 13

+++

## Functions can call other functions

- Function reusability is key results in cleaner code

- Reusing functions leverages key programming principle - **Don't Repeat Yourself**

- In the example of below, the surfaceAreaOfCube function **calls** another function (areaOfSquare) instead of duplicating work that was already done

```js

// Function that calculates area of a square

function areaOfSquare(side){
  return side * side;
};

areaOfSquare(3); // returns 9


// This is a function that calculates the 
// surface area of a cube that *reuses* the areaOfSquare function

function surfaceAreaOfCube(side){
  return 6 * areaOfSquare(side);
};

surfaceAreaOfCube(7); // returns 42

```


<a class="jsbin-embed" href="https://jsbin.com/yozuvij/embed?js,console">JS Bin on jsbin.com</a><script src="https://static.jsbin.com/js/embed.min.js?3.41.0"></script>


---
