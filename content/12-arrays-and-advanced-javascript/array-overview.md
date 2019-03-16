+++
date = "2017-01-22T18:04:24-05:00"
title = "Array Overview"
toc = true
next = "/12-arrays-and-advanced-javascript/anonymous-functions"
prev = "/12-arrays-and-advanced-javascript/agenda"
weight = 7

+++

## What are arrays?

- A collection of objects or items
- "Zero-based" - positions (called indexes) start at zero
- Very easy way to store multiple items
- Arrays can hold items of different datatypes (i.e. all items in an arry don't have to be the same datatype)
- Used extensively in programming

---

## Declaring an array

Two ways to declare an array

```js

// Declaring an empty array using the Array constructor syntax
var names = new Array();

// Declaring an empty array using literal notation (preferred)
var names = [];

// Declaring an array using literal notation with data
var names = ['larry', 'curly', 'moe'];

```

{{% notice tip %}}
The best practice is to use the literal notation whenever possible
{{% /notice %}}

---

## Arrays and Indexes

Arrays are "zero-based" meaning indexes start at 0

```js

  // the value 'curly' is said to have an index of 1
  var names = ['larry', 'curly', 'moe'];

```

---

## Getting data out of an array

The most common way to retrieve a single value from an array
is to use the index

```js

  var names = ['larry', 'curly', 'moe'];

  // retrieve the first item out of the array
  names[0]; // this wil return 'larry'

```

---

## More information about arrays

- Arrays one of the most useful data structures in programming, check our [MDN's documentation](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array) on Arrays for more information
