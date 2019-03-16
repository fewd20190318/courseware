+++
date = "2017-01-22T18:04:24-05:00"
title = "Flex Items Properties"
toc = true
next = "/06-flexbox/exercise"
prev = "/06-flexbox/flex-container-properties"
weight = 10

+++

![inline](/images/06/flex-items.svg)

## align-self

![inline](/images/06/align-self.svg)

- allows the default alignment (or the one specified by align-items) to be overridden for individual flex items.

```

.item {
  align-self: auto | flex-start | flex-end | center | baseline | stretch;
}


```

---

## Order

![inline](/images/06/order-2.svg)

- controls the order in which flex-items appear in the flex container


```

.item {
  order: <integer>;
}

```

---


## flex-grow

- defines the ability for a flex item to grow if necessary

- dictates what amount of the available space inside the flex container the item should take up

- a **unitless** measure that respresents a proportion or ratio

- flex-grow value **overrides the width of the flex-item**


```

.item {
  flex-grow: <number>; /* default 0 */
}

```

<a class="jsbin-embed" href="https://jsbin.com/ratecoc/embed?output">JS Bin on jsbin.com</a><script src="https://static.jsbin.com/js/embed.min.js?3.41.3"></script>

In the example above, the 2nd flex-item (green box) has its flex-grow set to 2 while the other flex-items have their flex-grow set to 1

----

## flex-shrink

- defines the ability for a flex item to shrink if necessary.

- a **unitless** measure that respresents a proportion or ratio (similar to flex-grow)

---


## flex-basis

- Controls the default size of an element, before it is manipulated by other Flexbox properties 

- It can be a length (e.g. pixels, percentages, etc) or auto

  - auto


```
.item {
  flex-basis: <length> | auto; /* default auto */
}

```



---

# flex shorthand

- allows developers to specify a flex-item's `flex-grow`, `flex-shrink` and `flex-basis` all at the same time


```

.item {
  flex: none | [ <'flex-grow'> <'flex-shrink'>? || <'flex-basis'> ]
}

```
