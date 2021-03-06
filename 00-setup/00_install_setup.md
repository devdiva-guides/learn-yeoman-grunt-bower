# Installation and Setup

You will need a command line application  in order to use these CLI tools

To take advantage of this modern, front-end development toolchain you will need to ensure that you system is setup with some decidedly old-school tools.  You will need:

* A terminal emulator (Terminal.app, iTerm, Console2, PowerShell etc.)
* _Optionally?_ Xcode Command Line Tools
* Node.js
* NPM (Node Package Manager)  _actually, this comes with node._
* Yeoman _this is actually installing three tools._
    * `yo`
    * `bower`
    * `grunt`


## Install

### Mac OS X

#### Install the XCode CLI Tools

*Prior to Mavericks* 
Either via Xcode > Preferences > Downloads

*Mavericks* 
Simply launch the terminal and type the following command:

```bash
xcode-select --install
```

Open your terminal and type the following commands to see if you already have any of the tools you need.  _You don't necessarily need to type all three commands to check for each tool._

```bash
yo
```

```bash
yo --version
```

```bash
which yo
```


```bash
bower
```

```bash
bower --version
```

```bash
which bower
```

```bash
grunt
```

```bash
grunt --version
```

```bash
which grunt
```

If you get a response for any of these, then it means you already have the tool you need installed.


Either download an installer package or use a package manager to install Node.js:

* http://nodejs.org/download/
* https://github.com/joyent/node/wiki/Installing-Node.js-via-package-manager

Test your installation to confirm you have node and npm.

```bash
node
```

```bash
node --version
```

```bash
which node
```

```bash
npm
```

```bash
npm --version
```

```bash
which npm
```


Follow the instructions for installing yeoman:

http://yeoman.io/learning/

```bash
npm install -g yo
```

_if your npm version < 1.2.10 then you will also have to install grunt and bower._

```bash
npm install -g grunt-cli bower
```



### Windows

__section is very draft__

<!-- 
Note: this is repetitive, probably need to restructure setup instructions:
* start with OS X vs Windows pre-reqs?
* or do separate tutorial for OS X / *nix versus Windows?
-->
Either download an installer package or use a package manager to install Node.js:

* http://nodejs.org/download/
* https://github.com/joyent/node/wiki/Installing-Node.js-via-package-manager

Follow the install instructions.


Once installed, you can launch the Node.js command shell.
Start > Programs > Node.js > Node.js

__Describe using node with cmd prompt, console2, hode.js shell, windows powershell, cygwin.  note any differences.__

http://dailyjs.com/2012/05/03/windows-and-node-1/


To launch the node.js REPL, simply type node in the command prompt. Success if the prompt changes to the node REPL.

```cmdprompt
node
```

Exit the REPL to return to the command prompt (ctrl-d to exit). Check if npm is setup correctly.  The following search should load npm and return matching search results.

```cmdprompt
npm search yo
```

Follow the instructions for installing yeoman:

http://yeoman.io/learning/

```bash
npm install -g yo
```

_if your npm version < 1.2.10 then you will also have to install grunt and bower._

```bash
npm install -g grunt-cli bower
```


## Setup

Chances are you already have a way of organizing your code projects on your computer.  I'm not going to mess with your setup... except to encourage you to have an consistent way of organizing your projects. By example, here is how I do it...

~/workspace  - this folder is where I have most of my code projects
~/workspace/oss - any open source projects
~/workspace/projects - actual work, clients, etc.
~/workspace/scratch -  tutorials, playing with different technologies

I'd encourage you to create something like a `scratch` folder where you can try stuff out without cluttering up your regular workspace areas.


```bash
cd ~/workspace/scratch
```

```bash
mkdir learn-yogrunt
```

```bash
cd learn-yogrunt
```

_if you want to get a little fancy on the command line. try flattening all of the above to the following._

```bash
mkdir -p ~/workspace/scratch/learn-yogrunt && cd ~/workspace/scratch/learn-yogrunt
```


You should see your command prompt's context change.  If in doubt, type `pwd` to print your working directory and confirm where you are.

You are ready to move on to the following "Hello World" exercises.

* Grunt - A basic setup
* Yeoman - Basic Scaffolding
