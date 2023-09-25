
## Can you change the state of a data structure using functional programming?

Yes, but not in the same way as you would in imperative programming. In functional programming, data structures are typically immutable, meaning that they cannot be modified once created. However, you can create new data structures that are derived from existing ones, and these new data structures can represent a changed state.

For example, you could create a function that takes a list and returns a new list with a new element added to the beginning. This function would not modify the original list, but it would create a new list that represents the changed state.


## Define purely functional programming.

Purely functional programming is a programming paradigm that treats all computation as the evaluation of mathematical functions.

## How do you think purely functional programming will differ from the programs you’ve written so far in this course?

The main difference between purely functional programming and the imperative programming  is that purely functional programming avoids mutable state. In imperative programming, it is common to use variables to store state and then modify that state over time. In purely functional programming, variables are typically used to represent immutable values, and any changes to state are made by creating new values.