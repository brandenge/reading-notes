
# Thinking in React and Higher Order Functions

## Thinking in React

### What is the single responsibility principle and how does it apply to components?



### What does it mean to build a ‘static’ version of your application?



### Once you have a static application, what do you need to add?



### What are the three questions you can ask to determine if something is state?



### How can you identify where state needs to live?



## Higher Order Functions

### What is a “higher-order function”?

A function that either takes another function as input, or returns another function as output, or both.

### Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?

Line 2 of the greaterThan function in the reading is returning an anonymous arrow function.

The call to greaterThan() assigns the parameter n in the function that it returns, so that function can be saved to a variable and then called again under the variable name. Calling the returned function using the variable name it was assigned to will assign the parameter m inside of the returned anonymous function.

This type of design to functions is sometimes useful when you need to create a bunch of functions all with very similar, but only slightly different logic to them.

Calling both functions at the same time using what looks like double-invoking parenthesis such as fn(a)(b) is called function currying.

### Explain how either map or reduce operates, with regards to higher-order functions.

map and reduce (and the other built-in array iterating methods) are higher order functions because they take a callback function as an argument. We can then think of these functions as being implemented with a traditional for-loop, where they call the callback function and pass in each element in the array as an argument to the callback function as it iterates through the array.

In the case of map, it creates a new array and returns it. In the case of reduce, it uses a variable that saves the returned value of the previous iteration through the array. This is very powerful and allows you to essentially replace any of the other built-in array iterating methods. This previous value variable can also be initialized to anything you want.
