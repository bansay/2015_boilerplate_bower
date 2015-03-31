## FRONTEND
## Grunt -> Compass Project Starter

## Theme Requirements (to compile with grunt):

* [Node.js](http://nodejs.org) Install Node first
* [Grunt](http://gruntjs.com) npm install -g grunt-cli
* [Bower](http://bower.io/) npm install -g bower

Installing gems requires that you have Ruby at least 1.8.3, to check you can run ruby -v
* [Sass](http://sass-lang.com) gem install sass
* [Compass](http://compass-style.org) gem install compass

## To ensure all the counterparts are installed, run

* sass -v
* npm -v
* compass -v
* bower -v

## Download Dependencies with Bower

1. run 'bower install' to install the dependencies (will read the bower.json file, and install into the _/lib directory, as defined on the .bowerrc file)

## To Compile SCSS with grunt:

1. cd into the themes' app directory, where the gruntfile.js and the package.json files are
    2. run 'npm install' to install the node_modules (including grunt and compass, as defined on the package.json in themes' app directory)
    2. run 'grunt' (default task for grunt, as defined on gruntfile.js in themes' app directory)
    3. run 'grunt dev' (task setup to run the watch task, as defined on gruntfile.js in themes' app directory)

## To Compile SCSS without npm/grunt/compass:

1. cd into the themes' app directory, where the gruntfile.js and the package.json files are
   a. inside the themes' app directory
    2. on _/scss/main.scss, comment out the @include 'compass' on main.scss
    3. run 'sass --watch _/scss/main.scss:_/css/main.css'