# Ready.js : continuous integration using jslint, nodejs and git

## What does it do?
1. Check if your javascript are valid with [jslint](http://www.jslint.com/).
2. Minify your javascript with [Closure Compiler](http://code.google.com/closure/compiler/) (optimize and minify your code).
3. Watch your javascript files for jslint while you're coding.
4. Create an aggregated file of all your javascripts.

## Prerequesites 

Install [git](http://git-scm.com/) and [node.js](http://nodejs.org/#download).

## How to install in your project (for git)

1. run `npm install ready`
3. Create config file in *your_project/ready.conf.js* :

        { src : "./javascripts", dest : "./minified" }
      
4. run `echo 'readyjs ready.conf.js' >> .git/hooks/pre-commit`

Then, **every time you commit**, ready.js will be run.

## How to watch your javascript files for errors with jslint

run `watchjs ready.conf.js`

## How to use ready.js
By installing with npm, you can call `readyjs` and `watchjs` like this :
    readyjs ready.conf.js

## Want to know more?

* [Alternatives installations](http://github.com/dsimard/ready.js/wiki)
* [Configuration options](https://github.com/dsimard/ready.js/wiki/Configuration-options)
* [FAQ](https://github.com/dsimard/ready.js/wiki/FAQ)



