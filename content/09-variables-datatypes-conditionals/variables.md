+++
date = "2017-01-22T18:04:24-05:00"
title = "Variables"
toc = true
prev = "/09-variables-datatypes-conditionals/console-log"
next = "/09-variables-datatypes-conditionals/data-types"
weight = 7

+++

## What are variables?

- Similar to algebra

- Helps you represent data or values

- Used to help your program “remember” values

- Can be thought of as a “box” that we put values in

- In programming, you store values in variables if you plan on referencing that value at a later time

---

## Declaring Variables

- Variables are created by **declaring** them

- Use the `var` keyword to declare a variable

- If you declare a variable without assigning it an initial value, the value of that variable will be **undefined**


```js

// declaring a variable

var firstName;

```

{{% notice tip %}}
  Variables **only need to be declared once**
{{% /notice %}}

---


## Assigning Variables

- We can provide variables with a value by **assigning** a value to the variable

- An `=` (equal sign) is used to assign a value to variable

```
// declaring a variable

var firstName;


// assigning a value to the variable

firstName = "Cletus";


```

---

## Declaring & Assigning Variables in one step

- We can both declare and assign variables in one step

- This would be done if the developer wanted to set the initial value of the variable


```js
// declare and assign an intial value to a variable

var score = 0;

```

---

## Reassigning a Variable

- Use the `=` (equal sign) to change or **reassign** a value of a variable


```

// declare and assign a value of 0 to the score variable
var score = 0;

// changing the value of the score variable from 0 to 3
score = 3;

```

---

## Variable Naming Rules

| Do                   | Don't                     |
|:----------------------|:-------------------------- |
| Use variable names that start with a letter, $, or _   | Use variable names that start with a number    | 
| Use variable names that includes letters, numbers, $ or _        | Create variable names that include a "-", "." or space       |  
| Use snake case when creating variable names made up of more than one word, for example: **firstName**       | Create variable names that use Javascript keywords such as **var**, **function** or **switch**                           | 

{{% notice tip %}}
  Variables names should describe the kind of information the variable stores
{{% /notice %}}


{{% notice tip %}}
  [Here's](https://mathiasbynens.be/notes/reserved-keywords) a list of Javascript's reserved keywords
{{% /notice %}}

