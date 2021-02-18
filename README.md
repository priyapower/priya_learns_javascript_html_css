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
## Part 4 - Vue CLI and To Do App
- **Environment:** I have a MacOS and my IDE is Atom. I am using the native Terminal on Mac.
- [Intro to Vue](https://v3.vuejs.org/guide/introduction.html)
- Vue is a progressive framework that helps you build user interfaces; the library focuses on the view layer (hence the name Vue!)
- Great for Single-Page Appllications (SPAs) OR integrating with other libraries/projects
- [Vue Hello World Example](https://codepen.io/team/Vue/pen/KKpRVpx)
- [To Do App Tutorial](https://scotch.io/tutorials/build-a-to-do-app-with-vue-js-2)
- Prerequisites:
  - [Node Package Manager](https://www.npmjs.com)
    - To [install](https://www.npmjs.com/get-npm)
  - [Vue Command Line Interface](https://cli.vuejs.org)
    - To [install](https://cli.vuejs.org/guide/installation.html)
  - **What I did:**, I already have `npm`, so I simply used `npm install -g @vue/cli`
  - **Terminal Output:**
    ```console
    /Users/priyapower/Coding/learning/frontend  $🐧npm install -g @vue/cli
    npm WARN deprecated request@2.88.2: request has been deprecated, see https://github.com/request/request/issues/3142
    npm WARN deprecated @hapi/joi@15.1.1: Switch to 'npm install joi'
    npm WARN deprecated @hapi/address@2.1.4: Moved to 'npm install @sideway/address'
    npm WARN deprecated @hapi/bourne@1.3.2: This version has been deprecated and is no longer supported or maintained
    npm WARN deprecated @hapi/topo@3.1.6: This version has been deprecated and is no longer supported or maintained
    npm WARN deprecated @hapi/hoek@8.5.1: This version has been deprecated and is no longer supported or maintained
    npm WARN deprecated har-validator@5.1.5: this library is no longer supported
    npm WARN deprecated resolve-url@0.2.1: https://github.com/lydell/resolve-url#deprecated
    npm WARN deprecated urix@0.1.0: Please see https://github.com/lydell/urix#deprecated
    npm WARN deprecated chokidar@2.1.8: Chokidar 2 will break on node v14+. Upgrade to chokidar 3 with 15x less dependencies.
    npm WARN deprecated fsevents@1.2.13: fsevents 1 will break on node v14+ and could be using insecure binaries. Upgrade to fsevents 2.

    > yarn@1.22.10 preinstall /usr/local/lib/node_modules/@vue/cli/node_modules/yarn
    > :; (node ./preinstall.js > /dev/null 2>&1 || true)

    /usr/local/bin/vue -> /usr/local/lib/node_modules/@vue/cli/bin/vue.js

    > fsevents@1.2.13 install /usr/local/lib/node_modules/@vue/cli/node_modules/fsevents
    > node install.js

    No receipt for 'com.apple.pkg.CLTools_Executables' found at '/'.

    No receipt for 'com.apple.pkg.DeveloperToolsCLILeo' found at '/'.

    No receipt for 'com.apple.pkg.DeveloperToolsCLI' found at '/'.

    gyp: No Xcode or CLT version detected!
    gyp ERR! configure error 
    gyp ERR! stack Error: `gyp` failed with exit code: 1
    gyp ERR! stack     at ChildProcess.onCpExit (/usr/local/lib/node_modules/npm/node_modules/node-gyp/lib/configure.js:351:16)
    gyp ERR! stack     at ChildProcess.emit (events.js:315:20)
    gyp ERR! stack     at Process.ChildProcess._handle.onexit (internal/child_process.js:277:12)
    gyp ERR! System Darwin 19.6.0
    gyp ERR! command "/usr/local/bin/node" "/usr/local/lib/node_modules/npm/node_modules/node-gyp/bin/node-gyp.js" "rebuild"
    gyp ERR! cwd /usr/local/lib/node_modules/@vue/cli/node_modules/fsevents
    gyp ERR! node -v v14.15.0
    gyp ERR! node-gyp -v v5.1.0
    gyp ERR! not ok 

    > core-js@3.9.0 postinstall /usr/local/lib/node_modules/@vue/cli/node_modules/core-js
    > node -e "try{require('./postinstall')}catch(e){}"

    Thank you for using core-js ( https://github.com/zloirock/core-js ) for polyfilling JavaScript standard library!

    The project needs your help! Please consider supporting of core-js on Open Collective or Patreon: 
    > https://opencollective.com/core-js 
    > https://www.patreon.com/zloirock 

    Also, the author of core-js ( https://github.com/zloirock ) is looking for a good job -)


    > @apollo/protobufjs@1.0.5 postinstall /usr/local/lib/node_modules/@vue/cli/node_modules/@apollo/protobufjs
    > node scripts/postinstall


    > nodemon@1.19.4 postinstall /usr/local/lib/node_modules/@vue/cli/node_modules/nodemon
    > node bin/postinstall || exit 0

    Love nodemon? You can now support the project via the open collective:
     > https://opencollective.com/nodemon/donate


    > ejs@2.7.4 postinstall /usr/local/lib/node_modules/@vue/cli/node_modules/ejs
    > node ./postinstall.js

    Thank you for installing EJS: built with the Jake JavaScript build tool (https://jakejs.com/)

    npm WARN @vue/compiler-sfc@3.0.5 requires a peer of vue@3.0.5 but none is installed. You must install peer dependencies yourself.

    + @vue/cli@4.5.11
    added 1407 packages from 714 contributors in 48.52s
    ```
  - **Confirm:** using `vue --version` I see `@vue/cli 4.5.11`
- The "out the box" packages that come with `Vue CLI` are:
  ```console
  webpack - A full-featured Webpack + Vue-loader setup with hot reload, linting, testing & CSS extraction.
  webpack-simple - A simple Webpack + Vue-loader setup for quick prototyping.
  browserify - A full-featured Browserify + vueify setup with hot-reload, linting & unit testing.
  browserify-simple - A simple Browserify + vueify setup for quick prototyping.
  simple - The simplest possible Vue setup in a single HTML file
  ```
 - **SO LET US GET STARTED!!**
- You can work with online IDE's like [JSFiddle](https://jsfiddle.net) or [Repl](https://repl.it), **however**, I enjoy working locally using my own IDE (in this case I am working with Atom (currently MacOS only), but there are plenty of great IDE's out there like VSCode and such)
- _Create a new project:_ First, I nagivated to the project pathway I desire my new project to be in (in my case: `/Users/<name>/Coding/learning_projects`). Then, in the terminal I use `vue init webpack todo-app` where `todo-app` is the name of my application/project
  - **UH OH** - I ran into an error
    ```console
    /Users/priyapower/Coding/learning/frontend  $🐧vue init webpack todo-app

    Command vue init requires a global addon to be installed.
    Please run npm i -g @vue/cli-init and try again.
    ```
- To fix this I ran `npm i -g @vue/cli-init`
  ```console
    /Users/priyapower/Coding/learning/frontend  $🐧npm i -g @vue/cli-init
    npm WARN deprecated vue-cli@2.9.6: This package has been deprecated in favour of @vue/cli
    npm WARN deprecated request@2.88.2: request has been deprecated, see https://github.com/request/request/issues/3142
    npm WARN deprecated coffee-script@1.12.7: CoffeeScript on NPM has moved to "coffeescript" (no hyphen)
    npm WARN deprecated har-validator@5.1.5: this library is no longer supported
    + @vue/cli-init@4.5.11
    added 251 packages from 206 contributors in 13.635s
  ```
-  Tried this command again: `vue init webpack todo-app` and I now see the prompts I expect
-  As each question is prompted, what is in the parenthesis represents what will default if you hit `enter`, otherwise begin typing to override and hit `enter` for the next prompt
  ```console
  ? Project name todo-app
  ? Project description An introductory Vue.js project
  ? Author Priya Power <49959312+priyapower@users.noreply.github.com>
  ? Vue build standalone
  ? Install vue-router? No
  ? Use ESLint to lint your code? Yes
  ? Pick an ESLint preset Standard
  ? Set up unit tests Yes
  ? Pick a test runner jest
  ? Setup e2e tests with Nightwatch? Yes
  ? Should we run `npm install` for you after the project has been created? (recommended) npm
  ````
- Once prompts were completed:
  ```console
     vue-cli · Generated "todo-app".


    # Installing project dependencies ...
    # ========================

    npm WARN deprecated babel-eslint@8.2.6: babel-eslint is now @babel/eslint-parser. This package will no longer receive updates.
    npm WARN deprecated eslint-loader@1.9.0: This loader has been deprecated. Please use eslint-webpack-plugin
    npm WARN deprecated extract-text-webpack-plugin@3.0.2: Deprecated. Please use https://github.com/webpack-contrib/mini-css-extract-plugin
    npm WARN deprecated browserslist@2.11.3: Browserslist 2 could fail on reading Browserslist >3.0 config used in other tools.
    npm WARN deprecated core-js@2.6.12: core-js@<3 is no longer maintained and not recommended for usage due to the number of issues. Please, upgrade your dependencies to the actual version of core-js@3.
    npm WARN deprecated request@2.88.2: request has been deprecated, see https://github.com/request/request/issues/3142
    npm WARN deprecated chokidar@2.1.8: Chokidar 2 will break on node v14+. Upgrade to chokidar 3 with 15x less dependencies.
    npm WARN deprecated bfj-node4@5.3.1: Switch to the `bfj` package for fixes and new features!
    npm WARN deprecated har-validator@5.1.5: this library is no longer supported
    npm WARN deprecated mkdirp@0.5.1: Legacy versions of mkdirp are no longer supported. Please update to mkdirp 1.x. (Note that the API surface has changed to use Promises in 1.x.)
    npm WARN deprecated json3@3.3.2: Please use the native JSON object instead of JSON 3
    npm WARN deprecated fsevents@1.2.13: fsevents 1 will break on node v14+ and could be using insecure binaries. Upgrade to fsevents 2.
    npm WARN deprecated browserslist@1.7.7: Browserslist 2 could fail on reading Browserslist >3.0 config used in other tools.
    npm WARN deprecated circular-json@0.3.3: CircularJSON is in maintenance only, flatted is its successor.
    npm WARN deprecated socks@1.1.10: If using 2.x branch, please upgrade to at least 2.1.6 to avoid a serious bug with socket data flow and an import issue introduced in 2.1.0
    npm WARN deprecated left-pad@1.3.0: use String.prototype.padStart()
    npm WARN deprecated request-promise-native@1.0.9: request-promise-native has been deprecated because it extends the now deprecated request package, see https://github.com/request/request/issues/3142
    npm WARN deprecated resolve-url@0.2.1: https://github.com/lydell/resolve-url#deprecated
    npm WARN deprecated urix@0.1.0: Please see https://github.com/lydell/urix#deprecated

    > fsevents@1.2.13 install /Users/priyapower/Coding/learning/frontend/todo-app/node_modules/fsevents
    > node install.js

    No receipt for 'com.apple.pkg.CLTools_Executables' found at '/'.

    No receipt for 'com.apple.pkg.DeveloperToolsCLILeo' found at '/'.

    No receipt for 'com.apple.pkg.DeveloperToolsCLI' found at '/'.

    gyp: No Xcode or CLT version detected!
    gyp ERR! configure error 
    gyp ERR! stack Error: `gyp` failed with exit code: 1
    gyp ERR! stack     at ChildProcess.onCpExit (/usr/local/lib/node_modules/npm/node_modules/node-gyp/lib/configure.js:351:16)
    gyp ERR! stack     at ChildProcess.emit (events.js:315:20)
    gyp ERR! stack     at Process.ChildProcess._handle.onexit (internal/child_process.js:277:12)
    gyp ERR! System Darwin 19.6.0
    gyp ERR! command "/usr/local/bin/node" "/usr/local/lib/node_modules/npm/node_modules/node-gyp/bin/node-gyp.js" "rebuild"
    gyp ERR! cwd /Users/priyapower/Coding/learning/frontend/todo-app/node_modules/fsevents
    gyp ERR! node -v v14.15.0
    gyp ERR! node-gyp -v v5.1.0
    gyp ERR! not ok 

    > chromedriver@2.46.0 install /Users/priyapower/Coding/learning/frontend/todo-app/node_modules/chromedriver
    > node install.js

    Current existing ChromeDriver binary is unavailable, proceding with download and extraction.
    Downloading from file:  https://chromedriver.storage.googleapis.com/2.46/chromedriver_mac64.zip
    Saving to file: /var/folders/ll/fyjn36hj0xq19gbf7csdgqq40000gn/T/2.46/chromedriver/chromedriver_mac64.zip
    Received 781K...
    Received 1568K...
    Received 2352K...
    Received 3136K...
    Received 3920K...
    Received 4704K...
    Received 5488K...
    Received 6272K...
    Received 6891K total.
    Extracting zip contents
    Copying to target path /Users/priyapower/Coding/learning/frontend/todo-app/node_modules/chromedriver/lib/chromedriver
    Fixing file permissions
    Done. ChromeDriver binary available at /Users/priyapower/Coding/learning/frontend/todo-app/node_modules/chromedriver/lib/chromedriver/chromedriver

    > core-js@2.6.12 postinstall /Users/priyapower/Coding/learning/frontend/todo-app/node_modules/core-js
    > node -e "try{require('./postinstall')}catch(e){}"

    Thank you for using core-js ( https://github.com/zloirock/core-js ) for polyfilling JavaScript standard library!

    The project needs your help! Please consider supporting of core-js on Open Collective or Patreon: 
    > https://opencollective.com/core-js 
    > https://www.patreon.com/zloirock 

    Also, the author of core-js ( https://github.com/zloirock ) is looking for a good job -)


    > uglifyjs-webpack-plugin@0.4.6 postinstall /Users/priyapower/Coding/learning/frontend/todo-app/node_modules/webpack/node_modules/uglifyjs-webpack-plugin
    > node lib/post_install.js

    npm notice created a lockfile as package-lock.json. You should commit this file.
    npm WARN ajv-keywords@2.1.1 requires a peer of ajv@^5.0.0 but none is installed. You must install peer dependencies yourself.

    added 1816 packages from 1118 contributors and audited 1822 packages in 35.16s

    44 packages are looking for funding
      run `npm fund` for details

    found 101 vulnerabilities (76 low, 9 moderate, 15 high, 1 critical)
      run `npm audit fix` to fix them, or `npm audit` for details


    Running eslint --fix to comply with chosen preset rules...
    # ========================


    > todo-app@1.0.0 lint /Users/priyapower/Coding/learning/frontend/todo-app
    > eslint --ext .js,.vue src test/unit test/e2e/specs "--fix"


    # Project initialization finished!
    # ========================

    To get started:

      cd todo-app
      npm run dev

    Documentation can be found at https://vuejs-templates.github.io/webpack
  ```
-  Following the "To get started" info, I can use `cd todo-app` followed by `npm run dev` (which will run development)
  - In the tutorial it asks us to run `npm install` (which installs dependencies), but in my prompts I selected the option to have it autorun this for me already, which is why I was able to skip this step
  - The output for `npm run dev`
    ```console
    /Users/priyapower/Coding/learning/frontend/todo-app  $🐧npm run dev

    > todo-app@1.0.0 dev /Users/priyapower/Coding/learning/frontend/todo-app
    > webpack-dev-server --inline --progress --config build/webpack.dev.conf.js

     12% building modules 24/28 modules 4 active ...earning/frontend/todo-app/src/App.vue{ parser: "babylon" } is deprecated; we now treat it as { parser: "babel" }.
     95% emitting                                                                        

     DONE  Compiled successfully in 3890ms                                                            3:49:43 PM

     I  Your application is running here: http://localhost:8080
    ```
  -  If I visit localhost 8080, I see:
  -  ![Welcome to your Vue App](https://user-images.githubusercontent.com/49959312/108432230-47332500-7201-11eb-8304-89169dc1f4bf.png)
  -  To exit the server in my terminal I use `CTRL + C`
-  Styling our application:
