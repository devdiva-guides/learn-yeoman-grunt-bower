# A Yeoman Hello World...

We are continuing the yeoman getting started instructions here:
http://yeoman.io/gettingstarted.html

Our goal is to make sure everything installed and works.  Not to mention, get a feel for the features.  As long as you don't get an error... this is all good!

```bash
mkdir -p ~/workspace/scratch/devmunch/using_grunt/000_setup/02_yo && cd  ~/workspace/scratch/devmunch/using_grunt/000_setup/02_yo

```

You should see your command prompt's context change.  If in doubt, type `pwd` to print your working directory and confirm where you are.

Install a yeoman generator to give it a whirl...

```bash
npm install -g generator-webapp
```

Once the generator is installed successfully, let's give it a whirl.


```bash
yo webapp
```

As you can see you are prompted by the generator to make some choice.  Try it out.  

Once you've made all your selections hit Enter to proceed.

Choose y|N when prompted to add libsass, hit Enter and watch the generator go!

We are not going to dig into everything that was created just now.  But review the output from the generator and/or list the files to take a look at everything that was done...

* Library choices enforced with some opportunity for configuration
* All the latest resources and dependencies you need to start  (scaffold) added in your app
* Note all the supporting code in your project's root and the "actual" code inside of `app`

## What else?

http://yeoman.io/faq.html

> How does Yeoman differ from Grunt?
>
> Yeoman builds upon a number of open-source tools to offer an opinionated workflow that helps developers achieve common tasks more easily. Grunt.js is one of these tools and powers our underlying build process and task plugin architecture.
>
> On top of this architecture, we've highly customized tasks, profiles and systems which work well together and also provide developers with features like our generator system and Twitter Bower integration. Yeoman takes care of configuring your Gruntfile and setup to support Sass, CoffeeScript and Require.js/r.js out of the box. With additional features like wiring, an improved serve and init, we like to think of ourselves as a helper project on top of Grunt.
>
> Developers are free to continue using any Grunt tasks with Yeoman and there should remain a good level of cross-tool task compatibility.Yeoman

## Yeoman's serve / live reload workflow

```bash
grunt serve
```

notice the output on the terminal. a bunch of tasks related to processing and serving our assets were run.  a livereload connection task started and a 'watch' task started and waiting for a triggering filesystem change event.

what else happened?
if you didn't notice it... the `grunt serve` task actually opened a browser window with our localhost server and app running in it.  with the livereload connection established, we can actually make changes to our code and see them update in the browser (without refereshing!)

Let's get less continental and change the home page's headline to "Hello, Hello!"

I'm going to make changes in the vi terminal editor.  You can do the same or open `app/index.html` in your favorite text editor.

we don't want to interup this process. so let's open a separate terminal window.   _note: for this type of workflow it's not uncommon to regularly have two terminal windows open._  You may need to change back to this directory if the new window didn't keep your location.

```bash
cd  ~/workspace/scratch/devmunch/using_grunt/000_setup/02_yo
```

```bash
vi app/index.html
```

Find "'Allo, 'Allo!" and replace with "Hello, Hello!"

Save your changes.

Observe.  What happened?
