+++
date = "2017-01-22T18:04:24-05:00"
title = "Flex Container Properties"
toc = true
next = "/06-flexbox/flex-items-properties"
prev = "/06-flexbox/flexbox-terminology"
weight = 9

+++

![inline](/images/06/flex-container.svg)

{{% notice note %}}
The upcoming (and awesome) gifs were graciously borrowed from [this insightful blog post](https://medium.freecodecamp.com/an-animated-guide-to-flexbox-d280cf6afc35#.rg3ffic99) that covers flexbox
{{% /notice %}}


## display

- Defines a flex container 

- inline or block depending on the given value

```css

.container {
  display: flex; /* or inline-flex */
}


```


![inline](/images/06/display-flex.gif)


---

## flex direction

![inline](/images/06/flex-direction2.svg)

- Establishes the main-axis and defines the direction flex items are placed in the flex container

- Determines whether the flex items are layed out as either horizontal rows or vertical columns


```css

.container {
  flex-direction: row | row-reverse | column | column-reverse;
}

```

![inline](/images/06/flex-direction.gif)

![inline](/images/06/flex-direction-column.gif)


---

## flex wrap

![inline](/images/06/flex-wrap.svg)

- flex-wrap allows developers to change that and allow the items to wrap as needed with this property


{{% notice tip %}}
By default, flex items will all try to fit onto one line
{{% /notice %}}

```css

.container {
  flex-wrap: nowrap | wrap | wrap-reverse;
}


```

---

## Flex Flow shorthand

- Allows developers to specify the `flex-direction` and `flex-wrap` properties at the same time

```

flex-flow: <‘flex-direction’> || <‘flex-wrap’>

```


```

//specifies flow-direction: row & flex-wrap: wrap
flex-flow: row wrap

```

---

## justify-content

![inline](/images/06/justify-content.svg)

- defines the alignment along the main axis

- will distribute extra free space left after all the flex items have reached their maximum size


```css

.container {
  justify-content: flex-start | flex-end | center | space-between | space-around;
}

```

![inline](/images/06/justify-content.gif)

---

## Align Items

![inline](/images/06/align-items.svg)

- defines the default behaviour for how flex items are laid out along the cross axis on the current line

![inline](/images/06/align-items.gif)

---

## Align Content

![inline](/images/06/align-content.svg)

- aligns a flex container's lines within when there is extra space in the cross-axis

- align-content **only applies when there are mutiple lines of flex items**


```css

.container {
  align-content: flex-start | flex-end | center | space-between | space-around | stretch;
}

```
