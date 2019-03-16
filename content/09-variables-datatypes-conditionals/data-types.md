+++
date = "2017-01-22T18:04:24-05:00"
title = "Data Types"
toc = true
prev = "/09-variables-datatypes-conditionals/variables"
next = "/09-variables-datatypes-conditionals/arithmetic-operators"
weight = 8

+++

## Strings

- Strings can consist of letters and other characters

- They are surrounded by either double quotes or single quotes

- Concatenation allows you to combine strings

```js
// declare a variable called color and store a string 

var color = "green";

```

{{% notice tip %}}
  Single or double quotes can be used for strings, but the opening quote must match the closing quote
{{% /notice %}}

---

## String Methods

- Javascript has some built-in methods that allow developers to work with strings

- For example: if you wanted to know how many characters were in a string, you would use the **.length** method

- Here are some example of other methods you can use on strings

<a class="jsbin-embed" href="https://jsbin.com/pataci/embed?js,console">JS Bin on jsbin.com</a><script src="https://static.jsbin.com/js/embed.min.js?3.41.0"></script>


{{% notice tip %}}
  [Click here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) for complete list of all the String methods
{{% /notice %}}


---

## Numbers

- Used for tasks involving counting or calculating sums

- Whole numbers (integers) or decimals (floats)

- Numbers can be negative or positive

- Numbers **do not have quotes around them**


{{% notice tip %}}
  There are no commas used when expressing numbers, for example the number 1,750 is expressed as 1750 in Javascript
{{% /notice %}}

<a class="jsbin-embed" href="https://jsbin.com/cosalon/embed?js,console">JS Bin on jsbin.com</a><script src="https://static.jsbin.com/js/embed.min.js?3.41.0"></script>


---

## Converting Strings to Numbers

- Sometimes you will find yourself in a position where you need to convert a string to a number

- This happens when you attempt to read numeric values from html (html displays everything as a string)

- Use the `parseInt()` or `parseFloat()` methods to accomplish this


<a class="jsbin-embed" href="https://jsbin.com/zutuji/embed?js,console">JS Bin on jsbin.com</a><script src="https://static.jsbin.com/js/embed.min.js?3.41.0"></script>

---

## Booleans

- Can only have a value of true or false 

- true/false are special keywords in javascript and **do not have quotes around them**

```js
// declare a variable called isOn and assign a value of true
var isOn = true;

// declare a variable called isWarm
var isWarm;

// assign a value of false to isWarm
isWarm = false;

```

- Booleans are useful for helping our programs make decisions (when used with conditionals, comparison & logical operators)

- Booleans also helps a program known when it should stop/start looping 

---

## Arrays

- Used to when you are working with a list of values that are related to each otehr

- Use square brackets to create an array

- Values in an array are separated by commas


---

## Creating an Array

- We can store variables just like any other data type

- You can create that doesn't initially contain any values, this is called an **empty array**

- An array can also be created with initial values

- Square brackets are a means of identifying if a variable is an array


```js

// declare a variable as an empty array

var numbers = [];

// or you can declare an array with initial values

var streets = ['Broadway', 'Houston', 'Grand'];

```

---

## Values in an Array

- Values in an array are accessed as if they are in a numbered list

- Arrays are **zero based** meaning the 1st “value” in an array is at position (index) 0, the 2nd element is at position 1, and so on

- You access the value of an element in the array by passing the index of the item in square brackets

```js

var streets = ['Broadway', 'Houston', 'Grand'];

// access the 2nd street listed in the array which is at index 1
var streetTwo = streets[1];

```

---

## Accessing  in an Array

- You can access a value of an array by referencing its **index** (i.e. its order within the array)

```js

// declare a variable called chipmunks and use it to store
// an array of names
var chipmunks = ["Alvin", "Simon", "Theodore"];

// reference the first value in the array
// here we pass in a zero, since that represents the first
// element (value) in an array

var bandMember = chipmunks[0];

// the value stored in bandMember is "Alvin"

```

---

## Changing Values in an Array

- You can change a value in an array by referencing the value and then changing the value using an `=` (equal sign) 

```js

// declare a variable called newEditionMembers and use it to store
// an array of names

var newEditionMembers = ["Ricky Bell", "Michael Bivins", "Bobby Brown", "Ronnie DeVoe", "Ralph Tresvant"]

// We are going replace Bobby Brown with Johnny Gill 
// by referencing the 3rd element of the array by using index 2
// and then use assignment (just an equal sign) to change
// the value to Johnny Gill

newEditionMembers[2] = "Johnny Gill";

```

---

## Array Examples

<a class="jsbin-embed" href="https://jsbin.com/wulexo/embed?js,console">JS Bin on jsbin.com</a><script src="https://static.jsbin.com/js/embed.min.js?3.41.0"></script>

{{% notice tip %}}
  Arrays are a flexible and powerful feature of Javascript (and other programming languages as well). [Click here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array) for more information about Arrays
{{% /notice %}}


---

## Objects

- Objects are used to represent real world objects in programming

- Within an object, variables are known as properties and functions are known as methods

- Curly braces are a means of identifying if a variable is an object


```js

// create an object that represents a dog

var myDog = {
	name: "Fido",
	age: 4,
	speak: function() {
     console.log('Woof woof');
	} 
}

```

- In the example above, we created an object and stored it in a variable called `myDog`

- This object has 2 properties (name and age) and 1 method (speak)


{{% notice tip %}}
	This of method as **actions** that our objects can take
{{% /notice %}}

----

## Accessing Properties and Methods of Objects

- Properties and values can be assigned and read using **Dot notation**

```js

var myDog = { 
  name: "Fido",
  age: 4,
  speak: function() {
     console.log('Woof woof');
	} 
}

// store myDog's name in a variable called dogName
var dogName = myDog.name;

// call the speak method of myDog 
myDog.speak();

```

<a class="jsbin-embed" href="https://jsbin.com/bumiwi/embed?js,console">JS Bin on jsbin.com</a><script src="https://static.jsbin.com/js/embed.min.js?3.41.0"></script>


---

## Updating Object properties using dot notation

- Object properties can be updated, added or deleted

<a class="jsbin-embed" href="https://jsbin.com/fupaxos/embed?js,console">JS Bin on jsbin.com</a><script src="https://static.jsbin.com/js/embed.min.js?3.41.0"></script>

{{% notice tip %}}
  This of method as **actions** that our objects can take
  Like arrays, objects are another flexible and powerful feature of Javascript. [Click here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object) for more information about Objects
{{% /notice %}}
