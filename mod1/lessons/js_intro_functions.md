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
  - Be able to declare functionws with and without parameters
  - Understand how to call functions with and without arguments
  - Make function expressions evaluate to something other than `undefined` using `return`
  - Understand and use operators and conditionals
- Vocabulary
  - `Function`: A predefined and reusable group of behavior
  - `Declare/Define`: The initial writing of a function
  - `Call/Invoke`: Running a function
  - `Parameters`: The variables declared when a function is declared/defined
  - `Arguments`: The variables passed to a function when it's called/invoked
- Anatomy of a Function/Invoking a Function/Passing Information to a Function
  - Functions are reusable blocks of code that group statements together to perform a specific task
  - Functions need a name, they can take parameters if needed using parenthesis, and then we use curly brackets to define where the statement for that function go
  - Typically, functions are named using action verbs
  - Function naming is camelCase
  - JS keyword to define a function is `function`
    ```js
    // Function without parameteres
    function makePizza() {
      var firstStatement = 'Pizza is AMAZING!';
      var pizza = "pepperoni";
      var secondStatement = "I love " + pizza + " pizza!";

      console.log(secondStatement);
      alert(firstStatement);
    }
    // Example of calling this function
    makePizza();
    ```
  - In the above example, the console will print "I love pepperoni pizza!" while the browser will display a pop up alert that says "Pizza is AMAZING!"
    ```js
    // Function with parameters
    function bakeCake(flavor, frosting, decoration) {
      return `I am baking a ${flavor} cake with ${frosting}. It will be decorated with ${decoration}.`
    }
    // Example of calling this function
    bakeCake("carrot", "cream cheese icing", "walnuts");
    ```
  - The second example will simply console print "I am baking a carrot cake with cream cheese icing. It will be decorated with walnuts."
- Parameters vs. Arguments
  - **Parameter**: The stipulated values that are declared in the function parenthesis location
  - **Argument**: The passed information when calling a function
  - Looking at the `bakeCake` function above: `(flavor, frosting, decoration)` are parameters, while `("carrot", "cream cheese icing", "walnuts")` are arguments
- Getting a Value from a Function BLARG BLARG BLARG BLARG
- The Return Statement
- Basic Conditional Structure
- ES5 vs ES6 Functions
