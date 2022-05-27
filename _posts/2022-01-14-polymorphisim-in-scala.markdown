---
layout: post
title: Polymorphism in Scala
description:
date: 2022-01-14 06:00:35 +0100
author: kamau
image: '/images/16.jpg'
tags: [scala, compSci]
tags_color: '#835F46'
---
# Polymorphism in Scala
### Introduction

As your code base grows and acquires more structure, it becomes necessary to introduce some abstraction to allows code reuse.
A basic form of abstraction that's ubiquitous in the standard library is the use of ADT **Abstract Data Type** is a data type whose representation is hidden from the client. 
A good example of an abstract data type is a priority queue. It can be represented In memory as an array, allocated cells on the heap, or in multiple other ways. 
Regardless of the underlaying implementation, it's abstracted over with a well defined interface defining the funcitons **push** and **pop**. You then call this functions to push items into the queue or pop the highest priority item without needing to know how the data type is actually implemented.

If you've written any non-trivial FP code, chances are you've come across a different kind of ADTs - **Algebraic Data Types**.

There's a difference between **Algebraic data types** and **Abstract data types**.

An algebraic data type is a type that consists of **sums** and **products**.(_see this article for more info_) whereas, an abstract data type is a data type that has its implementation abstracted over by a defined API.
The use of Abstract Data Types allow us to focus on the operations specified in the API rather that the actual implemenetaion or data representation.

So what does abstration have to do with polymorphism? well, alot. 

Polymorphism simply means having many shapes (**poly**: many, **morphisms**: shape). 
 
So going back to the kind of asbtraction we were talking about in the begining, immagine implementing a prority queue that can handle different types of data without having to change the implementation of the underlying funcitons.

There're a different kinds of polymorphisms but in this article we will concentrate on the three most comonly used in the Scala FP world.
- Parametric Polymorphism 
- Ad-hoc Polymorphism.

## Parametric Polyphorphism
If you've ever used generics in Java then you altready have a good grasp of what  parametric polymorphism is. 
Parametric Polymorphism is a feature of some type systems that allow us to write generic code. 

```scala
	trait PriorityQueue[T] {
		def push(t: T)
		def pop: T
	}
```
By adding one or more type variables to our type definition and using them in the type declaration (methods, fields, etc..) we end up with a polymorphic type.
Parametric polymorphism gets its name from the fact that we're introducing type variables as parameters.
So in our definition of PriorityQueue we introduce the type parameter T. The parameter is polymorphic because it can take multiple forms - it can take on many different types.

We could define a PriorityQueue which works with integers

```scala
	object StringQueue extends PriorityQueue[Int] {
		def push(t: Int): Unit = ???
		def pop: Int = ???
	}
```

So essentially, parametric polymorphism facilitates code reuse - which essentially boils down to the similarities across the different data structures and methods.



Type systems that allow a single piece of code to be used with multiple types
are collectively known as polymorphic systems.



# - \[DRAFT ~ WIP \] -
