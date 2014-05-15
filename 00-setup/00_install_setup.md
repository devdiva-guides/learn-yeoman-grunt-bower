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

Install the Xcode CLI Tools.  Either via Xcode > Preferences > Downloads or, _if you are using Mavericks_, simply launch the terminal and type the following command:

```
xcode-select --install
```

Open your terminal and type the following commands to see if you already have any of the tools you need.  _You don't necessarily need to type all three commands to check for each tool._

```bash
yo
yo --version
which yo
```


```bash
bower
bower --version
which bower
```

```bash
grunt
grunt --version
which grunt
```

If you get a response for any of these, then it means you already have the tool you need installed.


Either download an installer package or use a package manager to install Node.js:
* http://nodejs.org/download/
* https://github.com/joyent/node/wiki/Installing-Node.js-via-package-manager

Test your installation to confirm you have node and npm.

```bash
node
node --version
which node
```

```bash
npm
npm --version
which npm
```


Follow the instructions for installing yeoman:

http://yeoman.io/gettingstarted.html

```bash
npm install -g yo
```

_if your npm version < 1.2.10 then you will also have to install grunt and bower._

```bash
npm install -g yo
```



### Windows

_TODO add windows setup._


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
mkdir devmunch
```

```bash
cd devmunch
```

```bash
mkdir using_grunt
```

```bash
cd using_grunt
```

```bash
mkdir 000_setup
```

```bash
cd 000_setup
```


_if you want to get a little fancy on the command line. try flattening all of the above to the following._

```bash
mkdir -p ~/workspace/scratch/devmunch/using_grunt/000_setup && cd ~/workspace/scratch/devmunch/using_grunt/000_setup
```

You should see your command prompt's context change.  If in doubt, type `pwd` to print your working directory and confirm where you are.

You are ready to move on to the following "Hello World" exercises.

* Grunt - A basic setup
* Yeoman - Basic Scaffolding
