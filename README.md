# Codeschool - Shaping Up With AngularJS - Soup To Bits starting framework

This project is the starting code for [Codeschool](http://www.codeschool.com)'s screencast [Shaping Up With AngularJS - Soup To Bits](https://www.codeschool.com/screencasts/soup-to-bits-shaping-up-with-angular-js)


## Getting Started

To get you started you can simply clone the repository and install the dependencies.

### Prerequisites

You need git to clone the repository. You can get git from
[http://git-scm.com/](http://git-scm.com/).

We also use a number of node.js tools to install and initialize dependencies. You must have node.js and its package manager (npm) installed.  You can get them from [http://nodejs.org/](http://nodejs.org/).

### Clone the repository

Clone the repository using [git][git]:

```
git clone https://github.com/xipxoom/suwa-stb-framework.git
cd suwa-stb-framework
```

### Install Dependencies

We have two kinds of dependencies in this project: tools and angular framework code.  The tools help us manage and test the application.

* We get the tools we depend upon via `npm`, the [node package manager][npm].
* We get the angular code via `bower`, a [client-side code package manager][bower].

We have preconfigured `npm` to automatically run `bower` so we can simply do:

```
npm install -g bower
npm install -g http-server
npm install
```

Behind the scenes this will also call `bower install`.  You should find that you have two new
folders in your project.

* `node_modules` - contains the npm packages for the tools we need
* `app/bower_components` - contains the angular framework files

*Note that the `bower_components` folder would normally be installed in the root folder but angular-seed (the basis of this framework) changes this location through the `.bowerrc` file.  Putting it in the app folder makes
it easier to serve the files by a webserver.*

### Run the Application

We have preconfigured the project with a simple development web server.  The simplest way to start
this server is:

```
npm start
```

Now browse to the app at `http://localhost:8000`.

### Notes

I found it frustrating that the soup-to-bits screencast didn't have a fresh
starting point for beginning the project.  This code will sync up with about 14:08 in the video but I still **HIGHLY** recommend watching up until that point.

The video will still prompt you to copy code from the official finished app which can be found here:
https://github.com/codeschool/AngularJSSTB

This code is provided as-is with no support, guarantee, or warranty implied.  I have no official affiliation with AngularJS, angular-seed, or codeschool.

### Changes

* Removed dependencies in package.json and bower.json carried over from
angular-seed that were not needed for this course.

* Changed http-server to serve the app folder directly.

* Changed bower.json to also pull in bootstrap.

* Changed index.html to load boostrap.min.css from bower_components.
