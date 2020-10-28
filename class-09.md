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
