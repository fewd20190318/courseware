+++
date = "2017-01-22T18:04:24-05:00"
title = "Last Class Review"
toc = true
next = "/11-javascript-lab/lab-overview"
prev = "/11-javascript-lab/agenda"
weight = 7

+++

## What are Functions?

- Allows you to group a series of statements together to perform a specific task

- Functions are used to promote “code reuse”

- You can control when functions are executed, for example - you can write functions that only get executed (or called) when a user clicks a specific button



```js

// a simple function that greets you with a 'Good Morning' alert

// 1) Declare a function named greeting

function greeting(){
  alert('Good Morning');
};


// 2) Call (or run) the function

greeting();

```

---

## Declaring a Function

![inline](/images/10/declared_named_function_diagram.png)

- Use the `function` keyword to declare a function

- Functions can be given a name

- The name must be followed by parentheses

- The opening and closing curly braces indicate a “code block”

- The statements for your function goes within the code block

- Simply declaring the function **will not run this code**, this function must be “called” in order for the code inside the function to be run

---

## Calling a Function

![inline](/images/10/called_named_function_diagram.png)

- To run the code inside of a function you use the function name followed by parentheses (don’t forget the parentheses!)

- Now you can call this function as many times as you want

---

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

---

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
