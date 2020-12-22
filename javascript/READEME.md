# JavaScript

## Definitions/Jargon

- **declarative**: code that specifies what you want to do, without saying how
- **hoisting**: move all declarations to the top of the current scope or compiling phase, do not have to be initialized (default behavior)
- **imperative**: code that specifies how to do something
- **programming paradigm**: way to classify programming languages based on their features aka a bunch of rules to follow while writing code
- **side effects**: when code interacts with anything that could change the data in your program

## Functional Programming
[Resource](https://www.freecodecamp.org/news/functional-programming-in-javascript/)

- JavaScript is a multi-paradigm (declarative and imperative)
- Functional is a sub-paradigm of declarative programming
- Lots of built-in functions, often meaning less code
- Can be more abstract as you can just call a function without needing to know in depth what it does
- 2 laws:
1. Architect software with pure & isolated functions
Use a lot of:
- **pure function**: input gives same output, no side effects
- **idempotent function**: function that when you reapply results again it won't produce a different result
- **isolated function**: no dependence on state of program (including global variables)
- seems like a lot of restrictions but supposed to be guidelines to prevent bugs
- makes code more predictable
- easier to figure out what's happening
- doesn't matter execution order of code
- **first class function**: function that can be assigned to a variable
- all functions in JavaScript are first class functions
- **high order function**: function that takes a function as an argument and/or returns a function
- good for reusability
- i.e. `.map`, `.reduce`, `.filter`

2. Avoid mutability and side-effects
- **immutable**: unchanging over time
- if something has to change for your data structures, copy function then make changes

