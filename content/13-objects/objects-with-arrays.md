+++
date = "2017-01-22T18:04:24-05:00"
title = "Using Objects with Arrays"
toc = true
next = "/13-objects/code-along"
prev = "/13-objects/overview"
weight = 8

+++

## Objects with Arrays

- Since objects are used to represent real world "things", they are often combined with arrays to represent a collection of real world things


```
// declaring an array that contains objects as items

var shows = [
  { name: "Breaking Bad", genre: "Drama", network: "AMC" },
  { name: "Game of Thrones", genre: "Fantasy", network: "HBO" },
  { name: "Silicon Valley", genre: "Comedy", network: "HBO" },
  { name: "Narcos", genre: "Drama", network: "Netflix" },
  { name: "Vikings", genre: "Action", network: "History Channel" },
  { name: "Power", genre: "Drama", network: "Starz" },
];


```

- In the code example above, we have an array called `shows` that contains a collection of objects that represents some TV shows


## Looping (iteration) through an array of objects

- Looping through an array of objects is technically the same as looping through an array of any other datatype (i.e. strings, numbers, etc)


<a class="jsbin-embed" href="https://jsbin.com/lenuxax/embed?html,js,output">TV Shows on jsbin.com</a><script src="https://static.jsbin.com/js/embed.min.js?4.1.0"></script>


{{% notice tip %}}
  This example uses html tables, documentation for tables can be found [here](https://developer.mozilla.org/en-US/docs/Learn/HTML/Tables/Basics)
{{% /notice %}}
