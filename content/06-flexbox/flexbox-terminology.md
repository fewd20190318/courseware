+++
date = "2017-01-22T18:04:24-05:00"
title = "Flexbox Terminology"
toc = true
next = "/06-flexbox/flex-container-properties"
prev = "/06-flexbox/flexbox-overview"
weight = 8

+++

## Flexbox Terminology


![inline](/images/06/flex-terms.png)


### Flex Container

- The parent element in which flex items are contained

- Defined using the `flex` or `inline-flex` values of the **display** property

  - `flex`: will make the flex-container a block-level element

  - `inline-flex`: will make the flex-container an inline element

---


### Flex Item

- **Children of a flex container**


---

### Main Axis


- The axis along which the flex items follow each other

- `flex-direction` property determines the **main** axis

  
---


### Cross Axis 

- The axis perpendicular to the **main** axis


---

### Main Axis and Cross Axis changes with Flex Direction

- If the flex-direction is ``row`` or ``row-reverse`` then the **main axis** will be along the horizontal plane and the **cross axis** will be along the vertical plane

- If the flex-direction is ``column`` or ``column-reverse`` then the **main axis** will be along the vertical plane and the **cross axis** will be along the horizontal plane

