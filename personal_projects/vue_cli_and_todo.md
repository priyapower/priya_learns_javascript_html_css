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
