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
    - Shortcuts that I would practice with my Environment:
      - [Mac](https://macmost.com/printable-mac-keyboard-shortcut-page-for-macos-catalina.html)
      - [Spectacle - windows management](https://www.howtogeek.com/288124/how-to-rearrange-your-macs-windows-with-a-keyboard-shorcut/)
      - [Atom - Text Editor for Coding](https://www.bugsnag.com/blog/atom-editor-cheat-sheet)
      - [Mac Terminal](https://www.muo.com/tag/mac-terminal-commands-cheat-sheet/)
      - [Mac Chrome](https://i.pinimg.com/originals/40/dd/f9/40ddf9e7b7c28b6d892e8f3e04b449ff.png)
      - [Mac Chrome DEV TOOLS](https://i.stack.imgur.com/vx2Zs.png)
- [X] [Session 2](https://mod0.turing.io/session2/) and its [homework](https://gist.github.com/ericweissman/3e420f4c0290ed72b3881a45c8332b5e)
  - This covered:
    - Diving into `classes` with `attributes` and `methods`
    - Understanding file structures
    - Practicing using Command Line with Terminal
    - The basics of Git and version control
  - **This was completed during my time as a Turing student**
    - My notes on class `methods`:
      - Methods are the behaviors/actions that a class can have, like a `Pet` class having the ability to speak or a `Car` class can turn on a vehicle
    - My notes on File Structures:
      - _Files_ are the smaller object, the text docs, the images, videos, pdfs, etc. The thing you open on your computer when you click on a "file"
      - _Directories_ are the folders, where we organize files
      - A _File Path_ is the notation for where the file "lives" on your computer
      - Parent and Child are used to refer to rooted information, such as a directory called `Turing` may have directories inside of it called `Mod0` and `Mod1`. In this case the parent directory is Turing and the child directories would be Mod0 and Mod1. There is no limit to nesting - aka you can have multiple parents and children
    - My notes on Terminal/Command Line:
      - I use the `.zsh` shell ([bash vs zsh](https://scriptingosx.com/2019/06/moving-to-zsh/))
      - Commands to practice:
        - `pwd`: Print Working Directory - or, "Where am I?". This tells you what file path you are currently in
        - `mkdir <name_your_directory>`: Make Directory; creates a folder in the path you are currently in
        - `cd`: Change Directory; Move to the root directory if it is `cd` by itself
        - `cd <directory_name>`: Move into the director your specified if accessible from that path location
        - `cd ..`: Move back a level; you can nest this to go back multiple levels, for example, if I want to move back two levels I would use `cd ../..`
        - `ls`: List Directory - lists the contents of the directory your are in
        - `touch <file_name.filetype>`: Make a File
        - `cat`: Shows the contents of a file inside the terminal instead of opening it separately
        - `rm <file_name.filetype`: Remove a file
        - `rm -rf <directory_name>`: Remove a directory and all its contents
    - My notes on Git/Version Control
      - Version control is important because it lets us go back to previously working code or previous feature code; allows us to break our work into chunks that are accessible on different versions; work collaboratively inside group projects without overwriting other peoples work or breaking the code (or at least recognizing the break comes from the new code you are merging in); access to branches; access to tracking who made changes and when
      - Imagine you are working on a feature to add to a working product. You complete your work and you upload the information and now your product has a new feature. But... what if you have multiple people working on that new feature, perhaps all in the same file you are working in. Imagine 1000 people working on that same file. How do you ensure everyones work is tracked and accounted for? How do you ensure code isn't overwritten or destroyed? Version Control (and looking ahead, Continuous Integration) are resources that help us work on teams in effective ways
      - Commands to know:
        - `git init`: Initialize an empty git repository; this allows tracking to happen
        - `git clone <git_repository_information>`: This allows you to clone a git repository from "elsewhere" (GitHub is a common location to grab git initialized projects) onto your local computer; it will continue to track on your local as well
        - `git status`: let's you see what is being tracked by git; you may see untracked files or files added but not committed
        - `git add <file_name.filetype>`: Add a file to track in the "staging area"
        - `git add .`: Adds all files in untracked to tracked in the "staging area"
        - `git commit`: This allows you to write a commit message for the file(s) you have tracked; By itself, this command opens `Vim` world on the Terminal OR if you have setup your IDE and git configurations, it opens a similar file to the Vim editor in your IDE
          - While the Vim editor is easy enough to use, for beginners, I suggest getting comfortable with the command **below** before exploring the world of in-depth git commit messages
        - `git commit -m "<subject>"`: This is the commit message that let's us take the file(s) we added to our "staging area" and officially saving it to our version controlled repository; Think of this as a "snapshot in time" OR a "love letter to yourself/future-self/other-developers". These are notes that you can read to understand why code was added/updated/mutated/destroyed/etc. Remember to be clear and succinct - and always remember this is live information that may be visible to any and all. Leave a beautiful trail for others or your future self.
          - Example, a commit message of "Bug fixed" is... lacking. What about "Update product model for bug fix - changed attribute "height" from integer to float". Now we see that a bug fix happened and it most likely occurred because we needed access to decimal values. We could even go one step further and use the subject/body concept that many developers use:
            ```console
            Update product model for bug fix - changed attribute "height" from integer to float

            - While running test for calculating height dynamically, discovered a break in the code as I input float values versus integer values
            - Simple fix: change attribute datatype to Integer instead of Float
            - To ensure this bug is fixed, also added additional tests that test this feature using Floats instead of Integers
            ```
        - `git diff`: See the changes made to a file in comparison to the last saved version in the git repository
        - `git pull origin <branch_name>`: Grab the objects and refs from the branch you declared and integrate it within your local branch
          - This can potentially cause a `git merge` conflict error if your files don't quite match
        - `git push origin <branch_name>`: This pushes the committed information to the branch on the git repository
        - `git branch`: Lists the current branch you are on
        - `git branch -a`: Lists all branches in the git repo
        - `git checkout <branch_name>`: Move to the branch you named
        - `git checkout -b <new_branch_name>`: Create a new branch and move to it
    - My notes on
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
