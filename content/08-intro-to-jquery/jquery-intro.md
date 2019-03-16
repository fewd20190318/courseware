+++
date = "2017-01-22T18:04:24-05:00"
title = "Intro to jQuery"
toc = true
prev = "/08-intro-to-jquery/dom-intro"
next = "/08-intro-to-jquery/adding-jquery"
weight = 10

+++


## What is jQuery?

- A javascript library

- Offers a simple way to acheive a variety of common javascript tasks

- Consistent across all browsers

- Does not do anything pure javascript cannot do, just does it with a more intuitive syntax

---

## Benefits of jQuery?

- Uses CSS selectors

- Accomplishes more with less code

---

## CSS selectors means less code

```javascript

	// selecting an element using native/pure javascript
	document.getElementById('flavors');

```

vs

```javascript

	// using jQuery (same as above but with much more intuitive syntax)
	$('#flavors');

```

{{% notice tip %}}
  Use of CSS selectors to 'select' elements is one of the main reasons jQuery is so popular today
{{% /notice %}}

---

## CSS selectors means less code (continued)

```javascript

	// selecting an element using native/pure javascript
	document.getElementsByTagName('body')[0].style.backgroundColor = 'white';
```

vs 

```javascript

	// using jQuery (same as above but with much more intuitive syntax)
	$('body').css('backgroundColor', 'white');
```

{{% notice tip %}}
  Note: best practice is to use **camel case** when referencing css properties that have mutliple words i.e. 'backgroundColor' instead of 'background-color'
{{% /notice %}}


---

## Mental Model for using jQuery

1) Select an element using CSS selectors
2) Do something with that element using jQuery methods

```javascript

// selects an element with the id of 'flavor' and then
// adds the 'favorite' class to that element using 
// the addClass() method
$('#flavor').addClass('favorite');

```

---

## Documentation

You will be here very often so get familar with it!
## [api.jquery.com](http://api.jquery.com/)

