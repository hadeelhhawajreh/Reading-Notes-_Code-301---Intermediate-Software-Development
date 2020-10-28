Readings: FUNCTIONAL PROGRAMMING

*Concepts of Functional Programming in Javascript*

![img](https://miro.medium.com/max/875/1*JyVlvqwsCBYl2FuvPFVRZQ.png)

# What is functional programming?
Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data 

## Pure functions
The first fundamental concept we learn when we want to understand functional programming is pure functions. But what does that really mean? What makes a function pure?
So how do we know if a function is pure or not? Here is a very strict definition of purity:
It returns the same result if given the same arguments (it is also referred as deterministic)
It does not cause any observable side effects

It returns the same result if given the same arguments
Imagine we want to implement a function that calculates the area of a circle. An impure function would receive radius as the parameter, and then calculate radius * radius * PI:

  ``let PI = 3.14;``
  
``const calculateArea = (radius) => radius * radius * PI;``

``calculateArea(10); // returns 314.0``

Why is this an impure function? Simply because it uses a global object that was not passed as a parameter to the function.
Now imagine some mathematicians argue that the PI value is actually 42and change the value of the global object.
Our impure function will now result in 10 * 10 * 42 = 4200. For the same parameter (radius = 10)


Pure functions benefits

The code’s definitely easier to test. We don’t need to mock anything. So we can unit test pure functions with different contexts:
Given a parameter A → expect the function to return value B
Given a parameter C → expect the function to return value D

-----------------------------------------------------------------------
#### immutable

When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.
In Javascript we commonly use the for loop. This next for statement has some mutable variables.


+ toLowerCase: converts the string to all lower case
+ trim: removes whitespace from both ends of a string
+ split and join: replaces all instances of match with replacement in a given string


*pure functions + immutable data = referential transparency*

#### Higher-order functions
When we talk about higher-order functions, we mean a function that either:
takes one or more functions as arguments, or
returns a function as its result
The doubleOperator function we implemented above is a higher-order function because it takes an operator function as an argument and uses it.
You’ve probably already heard about filter, map, and reduce. Let's take a look at these.

##### Filter
Given a collection, we want to filter by an attribute. The filter function expects a true or false value to determine if the element should or should not be included in the result collection. Basically, if the callback expression is true, the filter function will include the element in the result collection. Otherwise, it will not.
A simple example is when we have a collection of integers and we want only the even numbers.

Imperative approach
An imperative way to do it with Javascript is to:
create an empty array evenNumbers
iterate over the numbers array
push the even numbers to the evenNumbers array
