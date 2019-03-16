+++
date = "2017-01-22T18:04:24-05:00"
title = "Working with Parameters"
toc = true
prev = "/10-functions/returning-values-from-functions"
next = "/10-functions/functions-calling-other-functions"
weight = 12

+++

## Declaring Functions that need information

![inline](/images/10/declared_named_function_with_parameters_diagram.png)

- Some functions need additional information in order to perform a specific task

- This additional information is referred to as “parameters”

- To provide parameters to a function, you specify them inside the parentheses after the parameter name

- The parameters are used like variables within the function body

- We use the “return” keyword when we want to retrieve a value from our function, in the case of the example we want to retrieve the result of the multiplying the width times the height

---

## Calling Functions that need information

```javascript

// Calling the getArea() function with values

getArea(7, 5); // returns 35


// Calling the getArea() function with variables

var doorWidth = 2;
var doorHeight = 8;

getArea(doorWidth, doorHeight); // returns 16

```

<a class="jsbin-embed" href="https://jsbin.com/meyovap/embed?js,console">JS Bin on jsbin.com</a><script src="https://static.jsbin.com/js/embed.min.js?3.41.0"></script>
