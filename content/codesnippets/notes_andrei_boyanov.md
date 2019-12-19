---
layout: default
title: Python Design Patterns - For Sleek and Fashionable Code
parent: python
nav_order: 3
---

# [Python Design Patterns: For Sleek and Fashionable Code](https://www.toptal.com/python/python-design-patterns)
Andrei Boyanov

## What is a design pattern?

**Design Patterns: elements of reusable and object-oriented software** by Erich Gamma, Richard Helm, Ralph Johnson, and John Vlissides (Gang of Four)

### 1. Program to an interface not an implementation

**duck typing:** "if it quacks, it's a duck".
don't care what the object is, only that it does what we want it to do

### 2. Favor object composition over inheritance
wrap a class in another class (???)

## Behavioral patterns
communications between objects.

Python has 11:  

1. [chain of responsibility](#chain-of-responsibility)
2. [command](#command)
3. interpreter
4. iterator
5. mediator
6. memento
7. observer
8. state
9. strategy
10. template
11. visitor

### chain-of-responsibility

> "target a request using different methods, each one addressing a sepcific part of the request"

> "every piece of code must do one thing and only one thing"

### command

(???) like history and undo?

## Creational Patterns
- not commonly used in python.
- because `python` is dynamic, you don't need the operator `new`

## Structural Patterns

### facade

interface object which exposes the user to only a subset of the functions.

### adapter

altering the interface.

> "Why alter well-tested code to support new interfaces when we can just implement an adapter that will translate the enw interfact to the well known one?"

### decorator

- introducing functionality without using inheritance
- wrap another function around an exisitng function.  
