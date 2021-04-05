# Lesson 1 - JS: Data Types & Variables

## Resources
- [Lesson source](https://frontend.turing.io/lessons/module-1/js-data-types-variables.html)
- [Scripting Languages](https://www.educative.io/edpresso/what-is-a-scripting-language)
- [MDN Docs - JS Data Types and Structures](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures)
- [Var, Let, and Const](https://codeburst.io/difference-between-var-let-and-const-in-javascript-fbce2fba7b4)

## My Notes
- Learning Goals
  - [ ] Be able to list the primitive data types used in JavaScript
  - [ ] Create and use variables to store values
  - [ ] Be able to add variables to strings (concatenation and interpolation)
- Vocabulary
  - Data Type: A kind of data, defined by the values it can hold and the operations that can be done on it
  - Primitive type: A kind of data type. Primitives in Javascript are [string, number, boolean, null, undefined, symbol]. Also know as a simple data type
  - Variable: A container for a value. The main building block for all programming
  - Declare: Creating a new variable (distinct from assignment)
  - Assignment: Assigning a value to a variable
  - Concatenation: The binding of multiple strings together using the + string operator
  - Interpolation: The process of injecting a variable directly into a string.
  - Template literal: Template literals are string literals that provide an easy way to interpolate a variable or expression into a string.
- What is Javascript
  - Makes the web more dynamic
  - It is a scripting language
    - Used to write scripts
    - A sereies of commands that are interperted one by one at runttime (vs programming languages that are compiled first before running)
    - JS tends to be a Client-side (user facing) scripting language
    - This means that it creates scripts that run on the client side (for example, a users browser)
    - Other client-side scripts might be jQuery, CSS
    - Server-side (connect with database) scripts might be Ruby, Perl, Python, PHP, etc
  - Most common language on the web
  - Since JS is so versatile and flexible, there are 100s of ways to accomplish the same task (Configuration over Convention)
- The Console
  - In Chrome you can access Dev Tools
    - Click view > developer > javascript console
    - Right click on site > inspect > console
    - Shortcut for console is CMD + OPTION + J
    - Shortcut for elements is CMD + OPTION + I)
- Data Types
  - 6 primitive data types
    - `Boolean` - logical entity - true or false
    - `undefined` - a variable that has not been assigneed a value
    - `null` - represents the intentional absence of any object value (treated as falsy)
    - `Number` (this is part of the numeric types) - 64 bit; represent typical numbers, including floating points. Has 3 symbolic values: `+Infinity`, `-Infinity`, `NaN` (Not a Number). There is also a number with 2 representations, `0` has both `-0` and `+0`. If you use `0`, you are also using `+0` since they are aliases.
    - `BigInt` (this is part of the numeric types) - You can safely store and operate on large integers beyond the safe integer limit for `Number`
    - `String` - represents textual data
    - `Symbol` - unique and immutable value that may be uses as the key of an `Object` property. Common synonym: atoms
  - Since JS is _loosely typed_ and _dynamic_:  Variables in JavaScript are not directly associated with any particular value type, and any variable can be assigned (and re-assigned) values of all types
- Saving and Naming Information with Variables
  - Variables help us store values for reuse
  - In JS, declaring a variable is typically 2 parts `var` (the special word that lets the interpretor know you are creating a variable) and then `variableNameDeclaration` (becomes the variable name)
  - For example: `var myVariableName;`
  - OR: `var myVariableName = "This is an example";`
  - Rules:
    - Names must begin with a letter, dollar sign($), or underscore(_)
    - Names can NOT begin with a number
    - Name can NOT contain a dash(-) or a period(.)
    - Name can NOT be reserved word like `var` or `for`
    - Names are case sensitive
    - Names should be descriptive of what the value is
    - Names are written in camelCase
- Re-assigning Values
  - You can always reassign a variable assigned using `var` by just redeclaring what is was set equal to. For example:
  ```js
  var age = 31;
  console.log(age); // 31
  age = 32;
  console.log(age); // 32
  ```
  - What about other keywords that allow variable assignment?
  - `var`
    - Function scoped (limited to the function; if outside function, global)
    - CAN be reassigned
    - ES5 version of a variable (older version; you will see this in production code, but there is a newer version)
  - `let`
    - Block scoped (limited to the block, aka the curly brackets)
    - CAN be reassigned
  - `const`
    - Block scoped (limited to the block, aka the curly brackets)
    - Can NOT be reassigned
- Using Variables Together
  - You can use **type coercion** in JS (Ruby won't allow the following examples type coercion)
  ```js
  // javascript type coercian example from number to string
  var quantity = 3;
  var mythicalCreature = " unicorns";
  var creatureCount = quantity + mythicalCreature;
  console.log(creatureCount); // "3 unicorns"
  ```
- Adding Variable Valus to Strings
  - Concatenation: Using the plus(+) symbol, you can combine different variables by lining them together
    ```js
    var quantity = 3;
    var mythicalCreature = "unicorns";
    var creatureCount = "I have " + quantity + " very fancy " + mythicalCreature;
    console.log(creatureCount); // "I have 3 very fancy unicorns"
    ```
  - Interpolation: You can add values to strings using **template literals**. In JS you use `${interpolatedVariable}`.
      ```js
      var quantity = 3;
      var mythicalCreature = "unicorns";
      var creatureCount = `I have ${quantity} very fancy ${mythicalCreature}`;
      console.log(creatureCount); // "I have 3 very fancy unicorns"
      ```
