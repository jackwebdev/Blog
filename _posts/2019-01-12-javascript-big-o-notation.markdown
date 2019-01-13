---
layout: post
title:  "JavaScript - Big O Notation"
date:   2019-01-12 014:01:17 GMT
category: Computer Science
image: "/Blog/assets/images/laptop.png"
# published: false
---
> This article isn't finished yet.

## What is it?
In simple terms, Big O Notation is a measurement that is used in order to determine the performance or complexity of an algorithm. As algorithm grows in complexity developers can use Big O Notation to work out the trends of time and space complexity of their algorithms. Big O Notation is a way to measure the "worst case" scenario of an algorithm and the trends rather than exact details.

### Time complexity
The measure of how long an algorithm takes to perform a task.

### Space complexity
The measure of how much memory is taken up while performing the task.

- **Linear**: The program will run for a time roughly proportional to the size of the input.
- **Quadratic / Exponential Runtime**: Doubling the size of the input will quadruple the run time.
- **Constant**: The program will run for the same length of time regardless of the input.
- **Logarithmic**: Doubling the size of the input will roughly result in fixed running time.

## Why do it?
A way of comparing algorithms performance trends, finding out how it will perform once you start using more data. How does it respond when you add increasing amounts of data?

## Expressions
The exact number of operations doesn't matter. Only the trends. I will explain the Big O classifications the best I can.

Let's start with the expression and how to read it. See the image below. 

![Breakdown of how the expression works](/Blog/assets/images/big_o_breakdown.png)

```javascript
console.log("Hello World!")
```

Above is a simple print statement. You might think that this is not exactly an algorithm, although as I see it any line of code that is completing a task can be defined as an algorithm. The complexity of this example is extremely low. In this example, this line of code would be known as a Big O Notation, `O(1)`. This expression in simple terms just means the algorithm will take the same number of elements. No matter the data input set, it will only take one step. Often known as being *Constant*.

Now, let's say we had an array filled with random words, and within that array want to search for a single letter "f". This would likely not be a Big O Notation, `O(1)` but an `O(n)`. `n` just means the number of elements or how many `n` times it takes to complete this algorithm. Big O Notation isn't specific and generalises. This represents an algorithm that will grow *Linearly* to the size of its input data set.


| Expression    | Definition                                                                                                               |                           
| ------------- |:------------------------------------------------------------------------------------------------------------------------:|
| `O(1)`        | Executes the same time regardless to the size of input data set.                                                         |
| `O(n)`        | Grows linearly in direct proportion to the size of its input data set.                                                   |                 
| `O(n²)`       | Performance is directly proportional to the square of the size of its input data set.                                    |                                               
| `O(log n)`    | Also known as log time.  Example: Binary search. Divides the structure in half and repeats until finds the exact number. |

## Logarithms
This is trickier to explain as it gets more into the maths side of things.
Definition taken from Google "A quantity representing the power to which a fixed number (the base) must be raised to produce a given number."

### Binary Search
This is a technique used to search sorted input data sets. It works by selecting the middle element, such as the median. An easier way I remember is where the search will keep halving the input data set until it grasps hold of the result and returns. This type of Algorithm is an example of `O(log N)`.


![Complexity Chart](http://i0.wp.com/www.jessicayung.com/wp-content/uploads/2016/08/screenshot-5.png?resize=846%2C591)
[src: bigocheatsheet.com](http://bigocheatsheet.com){:target="_blank"}