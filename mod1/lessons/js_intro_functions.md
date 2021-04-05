# Lesson 2 - JS: Intro to Functions

## Resources
- [Lesson source](https://frontend.turing.io/lessons/module-1/js-intro-to-functions.html)
- [Pre-work assignment](https://frontend.turing.io/lessons/module-1/js-statements-and-expressions.html)

## Pre-Work
- Learning Goals
  - Understand the difference between statements and expressions in Javascript
  - Use various operators in Javascript
- Vocabulary
  - `Statement`: A single piece of code that accomplishes one task or action
  - `Expression`: A statement that produces a value
  - `Operator`: Symbols that are used to assign, comapre, and perform operations
  - `Script`: A series of instructions that a computer can folow one-by-one
- Statements
  - The individual instructions in a script
  - Every statement is followed by a semicolon
    ```js
    "hello";
    358;
    false;
    console.log('BOOM');
    alert('POW');
    ```
- Expressions
  - As the browser reads each statement, if the result is a single value, we call this an expression
  - Expressions can use operators for a single value
    ```js
    "ap" + "ple"; // results in the expression "apple"
    2 + 3; // results in the expression 5
    ```
  - Expressions vs Statements: a statement tends to perform an action while an expression prduces a value
  - For example:
    - "It's raining a lot!" is a statement
    - "It's raining cats and dogs" is a statement, but more specifically, it is an **expression**
  - Or:
    - `4;` is a statement
    - `2 + 2;` is a statement AND an expression becuase it evaluates to 4
- Operators
  - Expressions rely on operators:
    - Assignment: assign a value to a variable using the equals(=) symbol; `var color = 'magenta';`
    - Arithmetic: perform basic math; `var addTwo = 2 + 2;`
    - String: combine strings; `var greeting = 'Hello! ' + 'Nice to meet you.';`
    - Comparison: compare 2 values and return true/false (inequalities from math); `var buy = 3 > 5; // Value of buy is false`
    - Logical: combines expressions and returns true/false; `var buy = (5 > 3) && (2 < 4);`

## My Notes
- Learning Goals
- Vocabulary
- Anatomy of a Function
- Invoke a Function
- Passing Information to a Function
- Parameters vs. Arguments
- Getting a Value from a Function
- The Return Statement
- Basic Conditional Structure
- ES5 vs ES6 Functions
