+++
date = "2017-01-22T18:04:24-05:00"
title = "Object Overview"
toc = true
next = "/13-objects/objects-with-arrays"
prev = "/13-objects/agenda"
weight = 7

+++

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
  Think of method as **actions** that our objects can take
  Like arrays, objects are another flexible and powerful feature of Javascript. [Click here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object) for more information about Objects
{{% /notice %}}
