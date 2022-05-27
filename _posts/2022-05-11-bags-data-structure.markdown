---
layout: post
title:  Bags data structure
date:   2022-05-11 07:00:00 +0100
author: kamau
image:  '/images/21.jpg'
tags:   [scala, compSci]
tags_color: '#618770'
---


# BAGS

A bag is a collection where removing items is not supported. Its purpose is to allow clients to collect and then iterate over items.
The order of the elements is unspecified and should be of no substantial consequence to the client.
You could use a stack or a queue in place of bag, but one way to emphasis that the order in which items are processed is irrelevant is to use a bag.

```scala
class Bag[T] extends Iterable[T] {
	private val ls = scala.collection.mutable.ListBuffer.empty[T]
	
	override def iterator: Iterator[T] = ls.iterator

	def push(t: T): Unit = ls.addOne(t)

	override def isEmpty: Boolean = ls.isEmpty

	override def size: Int = ls.size
}
```


# - \[DRAFT ~ WIP \] -