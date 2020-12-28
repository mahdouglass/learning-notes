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

## Unit Testing & Test Driven Development (Udemy Unit Testing and Test Driven Development in NodeJS)
### Why?
- Bugs hurt business
- Testing catches bugs before going to production
### Levels
- unit - function level (most comprehensive)
- component - library and compiled binary
- system - external intefaces of a system and it's sub-systems
- performance - sub-system and system to verify loading
### Unit Testing
- Safety net
- Tests individual functions - one for each function
- Positive/negative testing
- Executes in development environment
- Should be automated
- In unit test: describe test, have a setup, an action, and an assertion where it validates
### Test Driven Development (TDD)
- Process where developers take responsibility for quality of code
- Unit tests to be written before production code
- Shouldn't write all tests or production code at once
- Tests and production code are both written together in small bits of functionality
- Short cycle
- Immediate feedback
- Documents what code is doing
- Drives good object oriented design
- Tests should begin at the most simple of tests to more complicated
#### Work Flow
- Write a failing unit test (RED phase)
- Write basic production code to make test pass (GREEN phase) (update red phase to become green phase, not separate tests)
- Refactor unit test/production code to make it clean (REFACTOR phase)
- Repeat
#### Laws of TDD
- Don't write any production code until you have written a failing unit test
- Don't write more of a unit test than is sufficient to fail, and not compiling is failing
- Don't write more production code than is sufficient to pass the currently failing unit test
#### Example of tests descriptions
- Can I call function
- Get "1" when I pass in 1
- Get "2" when I pass in 2
- Get "Fizz" when I pass in 3
- Get "Buzz" when I pass in 5
- Get "FizzBuzz" when I pass in 15 or a multiple of 3
