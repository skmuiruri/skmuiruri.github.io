---
layout: post
title:  Arrays
date:   2022-04-15 06:39:00 +0100
author: kamau
image:  '/images/20.jpg'
tags:   [scala, compSci]
tags_color: '#666e76'
---
# Arrays
Arrays are mutable, indexed collections of values stored in contigous memory locations. 

Scala's arrays (**Array[T]**) correspond one-to-one with Java's arrays (**T[]**) but, offer much more than their java counterparts. 

Scala Array's are can be generic - so you can define a array **_Array[T]_** where **T** is a type parameter or an abstract type. 

## Creating Arrays
Arrays are zero based so 

If we have N values, we think of them as being numbered from 0 to N-1. Then, we can unambiguously specify one of them in Java code by using the notation a[i] to refer to the ith value for any value of i from 0 to N-1. This Java construct is known as a one- dimensional array.

Scala arrays are compatible with Scala sequences - you can pass an Array[T] where a Seq[T] is required. Finally, Scala arrays also support all sequence operations. 

# - \[DRAFT ~ WIP \] -