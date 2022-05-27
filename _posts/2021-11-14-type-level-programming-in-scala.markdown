---
layout: post
title: Type level programming
description: #
date: 2021-11-14 15:01:35 +0300
author: kamau
image: '/images/99.jpg'
tags: [scala]
tags_color: '#b25642'
---

# Type level programming

## Introduction

### Values vs Types

In scala, a value is anything that you can be correctly placed on the right side of the equals sign. 
So you can use both literals and expressions.
Values exist to store data.
Types exist only at compile time and are used by compilers to check the consistency of your program.
Types bind some value to a particular identifier that can be referenced inside a given scope. 

```scala
 type T = Int
```

Here we have a variable T that can hold some type. 

In scala values and types have different namespaces. So this means you have have a type and a value with the same name.

```scala
val t = 1
type t = Int

def fun(n: t): t = n
```

In reference to the code above, the scala compiler will know to differentiate between the value and the type even thought they have the same name.

Another useful way of viewing types is as a mathematical **set** of values, for instance you could think a Boolean as being a _set_ containing the values **true** and **false**.

[here](https://www.hackerrank.com/challenges/breaking-best-and-worst-records/problem)

### Implicits

### Type Classes
Type classes are a powerful tool used in functional programming to enable ad-hoc polymorphism. [rif](https://typelevel.org/cats/typeclasses.html)

Type systems that allow a single piece of code to be used with multiple types
are collectively known as polymorphic systems. [rif]
Polymorphism simply means having many shapes (Poly: many, morphisms: shape).

In scala, _type class_ is an abstract, parameterized type that lets us add new behavior to any closed data type without using sub-typing. [rif](https://docs.scala-lang.org/scala3/book/ca-type-classes.html#inner-main) 

# - \[DRAFT ~ WIP \] -