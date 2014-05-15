# A Grunt Hello World...

Read the Grunt getting started instructions for more details.

http://gruntjs.com/getting-started

Our goal is to make sure everything installed and works.  Not to mention, get a feel for the features.  As long as you don't get an error... this is all good!

```bash
mkdir -p ~/workspace/scratch/devmunch/using_grunt/000_setup/01_grunt && cd  ~/workspace/scratch/devmunch/using_grunt/000_setup/01_grunt

```

If the following command does not return a response, go back to 00_install_setup.sh

```bash
which grunt
```

First, let's generate the package.json file (metadata about your project). For now, use the defaults, simply hit Enter when prompted.

```bash
npm init
```

Add grunt to your project.

```bash
npm install grunt --save-dev
```

Observe. What happened?

A `node_modules` folder created.  Inside, all it contains for now is the  `grunt` module.

Let's try running grunt.

```bash
grunt
```

If grunt is working, you should get a response message with a fatal error.  Fortunately, it tells you exactly what is wrong... we need to create a Gruntfile (always named Gruntfile.js).

```bash
cat > Gruntfile.js
//Add Gruntfile declarations below
module.exports = function(grunt){
  // Project configuration

  // Default tasks
};
```

Let's log a message to the console with grunt.
```javascript
//Add Gruntfile declarations below
module.exports = function(grunt){
  // Project configuration

  // Default tasks
  grunt.registerTask('default',function(){
    console.log('Hello from grunt');
  });
};
```

Now, let's try to run grunt again.

```bash
grunt
```
