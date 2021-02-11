# Priya Learns Front End
----

## About
This repo represents a learning document as I further my skills in javascript, html, and css. Since I am a graduation of the Turing School of Software and Design (my main resource for learning), there may be sections that are addressed but not necessarily fully followed (which I will notate when that happens)

## Resources
- Started with the Turing School of Software and Design's [Mod 0 Foundation](https://mod0.turing.io)
- Following the Turing's [Mod 1 Front End Curriculum](https://frontend.turing.io)
- Using exercism's [Javascript track](https://exercism.io/my/tracks/javascript) for daily practice

## Part 0 - Setup
Resource: [Mod 0 Foundation](https://mod0.turing.io)
- [X] [Computer Setup](https://mod0.turing.io/setup-instructions)
  - This covered:
    - Feeling confident with the Mac
    - Installing Atom as IDE for the Mac
    - Installing Xcode-select for Mac
    - Installing Homebrew as a package manager for Mac
    - Installing Git for version control for Mac
    - Configuring Git on your local Mac
    - Installing Chrome
    - Configuring Atom for Terminal Access on Mac
    - Setting up GitHub account and adding GitHub SSH keys to your local Mac
  - **This was completed during my time as a Turing student**
    - I reviewed and ensured I had the correct and up to date environment
    - If you would like to see a general Windows setup - see here (link coming soon)
    - If you would like to see our Windows Sub System Linux setup - see here (link coming soon)
    - If you would like to see a Linux setup - see here (link coming soon)

## Part 1 - Turing Mod 0 Prep
- [X] [Session 1](https://mod0.turing.io/sessions/) and its [homework](https://gist.github.com/ericweissman/875e144c4d4334f9bdf04380d1211851)
  - This covered:
    - Note-taking
    - Googling
    - A basic introduction to `classes` and [`datatypes`](https://mod0.turing.io/session1/data-types-fe)
    - A brief practice with `markdown`
  - **This was completed during my time as a Turing student**
    - I feel confident with my notetaking. I prefer to use **_UpNote_** for my digital notes and a standard spiral notebook for my hand notes
      - My digital notes include copy and paste from lessons, code snippets, other digital resources
      - My physical notes might include drawings, visual aids, quick notes, anything else
      - I typically transfer all physical notes to the digital section on UpNote after a lesson
    - I also feel confident with my googling skills - a skill I honed as an online undergraduate as well as in my time as a public school teacher
    - My personal notes on Classes
      - A `class` is a category that we can then make an `instance` of
        - For example: We could have a `Desk` class with examples of the instances being a `standing desk` versus a `l-shaped desk`.
      - Class names are singular
      - Class names are `PascalCase` - every first word is capitalized with no spaces between words, such as `IAmInPascalCase`
      - Class attributes are the characteristics that every single instance will also have
        - For example: Looking back at our `Desk` class, we might declare attributes like `style`, `height`, `width`, `length`, `number_of_legs`, etc...
    - My personal notes on Datatypes in Javascript
      - Variable Assignment:
        - Use `var` to declare a variable
        - Write the variable name in `camelCase` - besides the first word, every word is capitalized with no space between words, such as `thisIsInCamelCase`
        - Set the new variable equal to whatever datatype you would like
        - Close the statement with a semi-colon
        - `var variableName  = 5;`
        - **Remember that naming should be representation of what the variable represents - be clear and succinct**
      - String: represents text; defined with quotation marks such as `var string1 = "This is a test string";`
      - Number: In javascript, there is no distinct difference between an Integer and a Float, they are all the number datatype. However, it is important to know these differences in other languages:
        - Integer: represents a whole number such as `var int1 = 10;`
        - Float: represents a floating point - aka number values with decimal points such as `var float1 = 99.32;`
      - Boolean: represents true/false such as `var boolean1 = true;`
      - Array: represents a group of things; defined with square brackets such as `var array1 = [1, 2, 3];` or `var fruitsInMyFridge = ["orange", "banana", "grape", "apple", "strawberry"];`
      - Object/Dictionary: represents a group of key:value pairs; similar to an array since it is a collection of info, however, here we can pair data together; defined with curly brackets, such as `var object1 = {key: value, key2: value2, key3: value3};` or
      ```javascript
      var mealTimesForHobbits = {
        breakfast: "7:30 AM",
        secondBreakfast: "9:00 AM",
        elevensies: "11:00 AM",
        luncheon: "12:30 PM",
        afternoonTea: "2:00 PM",
        dinner: "5:30 PM",
        supper: "8:00 PM"
      };
      ```
    - My personal notes on Datatypes in Ruby
      - Even though this learning document is focused on FE, I thought it would be nice to see a comparison
      - Variable Assignment:
        - In Ruby, we don't need any preface to declare a variable
        - Write the variable name in `snake_case` - all words are lowercase with an "_" between words, such as `this_is_in_snake_case`
        - Set the new variable equal to whatever datatype you would like
        - No closing required in Ruby
        - `variable_name  = 5`
        - **Remember that naming should be representation of what the variable represents - be clear and succinct**
      - String: represents text; defined with quotation marks such as `string_1 = "This is a test string"`
      - Integer: represents a whole number such as `integer_1 = 10`
      - Float: represents a floating point - aka number values with decimal points such as `float_1 = 99.32`
      - Boolean: represents true/false such as `boolean_1 = true`
      - Array: represents a group of things; defined with square brackets such as `array_1 = [1, 2, 3]` or `fruits_in_my_fridge = ["orange", "banana", "grape", "apple", "strawberry"]`
      - Hash: represents a group of key:value pairs; similar to an array since it is a collection of info, however, here we can pair data together; defined with curly brackets; Ruby has something interesting as that they key can be a `number`, `word`, or `symbol` as long as they are unique to that hash; In Ruby, you use the "hash rocket" (=>) to declare key:value pairs, such as:
      ```ruby
      # String Hash Keys
      hash_with_string_keys = {"key" => "value", "key2" => "value2", "key3" => "value3"}
      # Number Hash Keys
      hash_with_string_keys = {1 => "value", 2 => "value2", 3 => "value3"}
      # Hash with symbols as keys
      meal_times_for_hobbits = {
        :breakfast => "7:30 AM",
        :secondBreakfast => "9:00 AM",
        :elevensies => "11:00 AM",
        :luncheon => "12:30 PM",
        :afternoonTea => "2:00 PM",
        :dinner => "5:30 PM",
        :supper => "8:00 PM"
      }
      # New Ruby versions allow auto creation of symbols using shorthand and removing the "rocket symbol"
      meal_times_for_hobbits = {
        breakfast: "7:30 AM",
        secondBreakfast: "9:00 AM",
        elevensies: "11:00 AM",
        luncheon: "12:30 PM",
        afternoonTea: "2:00 PM",
        dinner: "5:30 PM",
        supper: "8:00 PM"
      }
      ```
- [X] [Session 2](https://mod0.turing.io/session2/) and its [homework](https://gist.github.com/ericweissman/3e420f4c0290ed72b3881a45c8332b5e)
  - This covered:
    - Diving into `classes` with `attributes` and `methods`
    - Understanding file structures
    - Practicing using Command Line with Terminal
    - The basics of Git and version control
  - **This was completed during my time as a Turing student**
- [X] [Session 3](https://mod0.turing.io/session3/) and its [homework](https://gist.github.com/ericweissman/92594fbd254208c2922443fdd21d6ba5)
  - This covered:
    - Practicing shortcuts in Terminal and Atom
    - Practicing classes and methods
    - Practicing Git
    - Understanding GitHub, Repositories, Forking, and Cloning
  - **This was completed during my time as a Turing student**
- [X] [Session 4](https://mod0.turing.io/session4/) and its [homework](https://mod0.turing.io/session4/#assessmentprev)
  - This covered:
    - Understanding what **Driver-Navigator** relationship is when paired coding
      - The **Driver** is the person whose screen is shared. Their behavior: listen to the navigator for instructions, ask for clarity as needed, and be the person who codes/types/writes/moves on the screen
      - The **Navigator** is the person who is watching the screen share. Their behavior: guide the driver with clear and precise instructions, respond to questions from the driver, and be the person who walks the coder through the instructions.
    - Practicing the Driver-Navigator relationship
    - An intro to Object Oriented Programming (OOP)
    - Understanding Turing's Mod 0 Assessment with a practice assessment
  - **This was completed during my time as a Turing student**
1. [X] [Session 5](https://mod0.turing.io/session5/)
  - This covered:
    -
  - **This was completed during my time as a Turing student**

## Part 2 - Leaving Mod 0 Entering Mod 1 Prework
## Part 3 - Exercisms: Hello World, Two Fer, Resistor Color, and Resistor Color Duo
