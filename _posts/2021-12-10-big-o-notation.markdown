---
layout: post
title:  Big-O notation
description: The Big-O notation
date:   2021-12-10 04:01:35 +0100
author: kamau
image:  '/images/17.jpg'
tags:   [compSci]
tags_color: '#477690'
---
# Big-O notation for developers

**Big O notation** is a system for measuring the rate of growth of an algorithm.

Big O notation provides us a common language that we can use to talk about the complexity of algorithms. Its a notation for measuring the complexity of an algorithm in terms of **space** and **time**.

Its common among developers (mostly novice developers) to measure the time an algorithm takes in seconds or milliseconds. This approach is quite limited because it reveals the velocity of an algorithm in a very particular context but it says nothing about the behaviour of the algorithm when the context changes.

What we really want to know is the **rate of growth** of the algorithm - how many operations it takes to complete.

The **O** in Big-O is actually the greek letter ***Omicron*** which means **order of**. 
So when we say that an algorithm is **O(n)** what it means is that the **order of** (_rate of growth_) of that algorithm is n.

Big-O annotation is used to define the worst case scenario or the the **upper bound**.

Algorithms can have diffent orders of complexity:

|    			| Complexity  |
|---------------|-------------|
| O(1)   		|  constant 
| O(n)   		|  liner	  
| O(n^2)  		|  quadratic 
| O(log n)  	|  logarithmic
| O(n * log n)  |  log linear 
| O(n^3)  		|  cubic 
| O(2^n)  		|  Exponential 
| O(n!)  		|  Factorial 


## O(1) - Constant Time Complexity
Some algorithms only need to run just one operation to return the desired value. A good example is accessing a map. Given a key, you can access the corresponding value directly without having to view any other element in the collection.
This type of complexity is reffered to as being constant because it does not changa regardless of the size of the map.

One way of checking whether your algorithm's complexity is **O(1)** is by confirming that he input provided does not affects the number of operations performed.

So when you have a rate of growth of **O(1)**, also called _constant time complexity_, the size of your input will not impact the number of operations performed.


## O(n) - Linear Time Complexity
With a rate of growth of O(1) or constant time, the number of operations remain the same regardless of the input. With linear time complexity, the rate of growth scales in direct proportion to the input provided. 
Remember, Big-O is all about worst case scenarios so with O(n) complexity, the number of operations performed might actually be less than n but the worst case scenario will be n operations.

## O(n^2) - Quadratic Time Complexity
While the number of operations in Linear complexity is in direct proportion to the input, the number of operations in a quadratic complexity is in proportion to the square of the input ~ so input to the power of 2. 
Any power beyond 2 is said to be **exponential** complexity.

A typical example of an algorithm of quadratic complexity is a loop nested inside another loop.

# - \[DRAFT ~ WIP \] -