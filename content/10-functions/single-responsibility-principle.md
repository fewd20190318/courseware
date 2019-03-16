+++
date = "2017-01-22T18:04:24-05:00"
title = "Single Responsibility Principle"
toc = true
prev = "/10-functions/code-along-1"
next = "/10-functions/code-along-2"
weight = 15

+++

## Single Responsibility Principle (SRP)

- SRP is a programming best practice that advocates **modular** code

- Put another way, your programs should be broken up in such a way where each part is responsible for only one "thing" or domain

- SRP is often applied to functions


## Applying SRP to Functions

- This concepts calls for your functions to only be "responsible" for one thing

- Often you'll find that the logic in your functions are doing too much (for example: making calculations AND displaying the result to the screen)

- In these cases you should break out those multiple responsibilities into multiple functions

- This is what we did in the Geometry Calculator code along
