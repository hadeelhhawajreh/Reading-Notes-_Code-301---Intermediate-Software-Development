Read: 06 - Node, Express, and APIs

![node](https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcTVDr1CDWrGTbhynAQgD1XQaaQ1STQwscn6JQ&usqp=CAU)


*What Is Node.js?*
Node.js is an event-based, non-blocking, asynchronous I/O runtime that uses Google's V8 JavaScript engine and libuv library. It is used for developing applications that make heavy use of the ability to run JavaScript both on the client, as well as on server side and therefore benefit from the re-usability of code and the lack of context switching.

>Node.js® is a JavaScript runtime built on Chrome’s V8 JavaScript engine.

![im](https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcQyRD66lLUXfIClcTAduy_PTV9EHnrUDLagEQ&usqp=CAU)


*Node Is Built on Google Chrome’s V8 JavaScript Engine*
The V8 engine is the open-source JavaScript engine that runs in Google Chrome and other Chromium-based web browsers, including Brave, Opera, and Vivaldi. It was designed with performance in mind and is responsible for compiling JavaScript directly to native machine code that your computer can execute.

![img](https://developer.ibm.com/developer/default/tutorials/learn-nodejs-tour-node/images/figure-1.png)

#### Applications that can be written using Node.js include, but are not limited to:
+ Static file servers
+ Web Application frameworks
+ Messaging middleware
+ Servers for HTML5 multi player games, or streaming audio/video
+ Real time applications
+ Cross-platform programs

#### How Do I Install Node.js?
In this next section, we’ll install Node and write a couple of simple programs. We’ll also look at npm, a package manager that comes bundled with Node


Working with the package.json File
If you look at the contents of the test directory, you’ll notice a folder entitled node_modules. This is where npm has saved lodash and any libraries that lodash depends on. The node_modules folder shouldn’t be checked in to version control, and can, in fact, be re-created at any time by running npm install from within the project’s root.

If you open the package.json file, you’ll see lodash listed under the dependencies field. By specifying your project’s dependencies in this way, you allow any developer anywhere to clone your project and use npm to install whatever packages it needs to run.

**What Is Node.js Used For?
Now that we know what Node and npm are and how to install them, we can turn our attention to the first of their common uses: installing (via npm) and running (via Node) various build tools — designed to automate the process of developing a modern JavaScript application.**

These build tools come in all shapes and sizes, and you won’t get far in a modern JavaScript landscape without bumping into them. They can be used for anything from bundling your JavaScript files and dependencies into static assets, to running tests, or automatic code linting and style checking
