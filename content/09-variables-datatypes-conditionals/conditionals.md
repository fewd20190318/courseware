+++
date = "2017-01-22T18:04:24-05:00"
title = "Conditionals"
toc = true
prev = "/09-variables-datatypes-conditionals/logical-operators"
next = "/09-variables-datatypes-conditionals/code-along-3"
weight = 13

+++

## What are Conditionals?

- Condtionals tests whether an “expression” evaluates to true or false and then makes a decision based on the results of that test

- **if statements** are the most common form of conditionals

- There are two types of if statements

	- (if else) statements

	- (if else if) statements


---

## (if else) statements

- when evaluating between just two choices, use if/else

- These are great for “either or” situations

- You **do not specify a condition** for the “else” clause


```js

var brushedTeeth = false

if(brushedTeeth){

  alert('Great job, you brushed your teeth!');

} else {

  alert('Go your brush teeth man, your breath is hot right now!');
}

```

<a class="jsbin-embed" href="https://jsbin.com/bofidag/embed?js,console">JS Bin on jsbin.com</a><script src="https://static.jsbin.com/js/embed.min.js?3.41.0"></script>


---

## (if else if) statements

- when evaluation among more than two choices, use if/else if

- You must specify a condition on the “else if” clause


```js

var yourGrade = 84;

if (yourGrade >= 90) {

  alert("Congrats your score is 90 or above, that's an A!");

} else if (yourGrade >= 80){

  alert("Congrats your score is 80 or above, you earned a B");

} else {

  alert("Your score is less than 80, no bueno");
}

```

<a class="jsbin-embed" href="https://jsbin.com/relane/embed?js,console">JS Bin on jsbin.com</a><script src="https://static.jsbin.com/js/embed.min.js?3.41.0"></script>
