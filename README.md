
     _____  _    _          _   __               _   __                             __       _    
    |_   _|/ |_ | |        / |_[  |             / |_[  |                           [  |     / |_  
      | | `| |-'\_|.--.   `| |-'| |--.  .---.  `| |-'| |--.   .--.   __   _   .--./)| |--. `| |-' 
      | |  | |    ( (`\]   | |  | .-. |/ /__\\  | |  | .-. |/ .'`\ \[  | | | / /'`\;| .-. | | |   
     _| |_ | |,    `'.'.   | |, | | | || \__.,  | |, | | | || \__. | | \_/ |,\ \._//| | | | | |,  
    |_____|\__/   [\__) )  \__/[___]|__]'.__.'  \__/[___]|__]'.__.'  '.__.'_/.',__`[___]|__]\__/  
      _   __              _                                      _          ( ( __))              
     / |_[  |            / |_                                   / |_                              
    `| |-'| |--.   ,--. `| |-'  .---.   .--.   __   _   _ .--. `| |-'.--.                         
     | |  | .-. | `'_\ : | |   / /'`\]/ .'`\ \[  | | | [ `.-. | | | ( (`\]                        
     | |, | | | | // | |,| |,  | \__. | \__. | | \_/ |, | | | | | |, `'.'.  _                     
     \__/[___]|__]\'-;__/\__/  '.___.' '.__.'  '.__.'_/[___||__]\__/[\__) )(_)                    
                                                                                              
    ----------------------------------------------------------------- 


# `Makeme` - A Universal Javascript generator for #coolkids 
`Makeme` is a universal javascript stack generator for Yeoman - featuring Angular, Express, Node, Mongo and Socket. 

[ ![Codeship Status for giftstarter/generator-makeme](https://codeship.com/projects/434a9b80-90b9-0133-623b-4e0b09ec4af6/status?branch=master)](https://codeship.com/projects/124478)

> Are you looking for [**`Makeme Famous`**](https://www.github.com/giftstarter/generator-makeme-famous)? 

## GyShiDo with `makeme`
To get shit done, here's a quick list of useful info. 

#### Table of Contents

1. [Universal Javascript](#Welcome-to-Universal-Javascript) with Angular
2. [Setting Up](#setting-up)
3. [Supported Configurations](#supported-configurations)
4. [Project Structure](#project-structure)
5. [Typical workflows](#typical-workflows)
6. [Gulp tasks](#gulp-tasks)
7. [Bower components](#bower-components)
8. → [Generators](./app/templates/docs/generators.md) docs 
9. → [Testing](./app/templates/docs/testing.md) docs
10. → [Deployment](./app/templates/docs/deploy.md) docs
11. [Changelog](#changelog)
12. [Upgrade](#upgrade)

<img src="http://yeoman.io/static/illustration-home-inverted.1f863f34ba.png" width="500px">

---

<img src="http://www.w3schools.com/angular/pic_angular.jpg" width="50px"><img src="https://supundharmarathne.files.wordpress.com/2013/08/nodejs.png" width="50px"><img src="http://www.codingpedia.org/wp-content/uploads/2014/04/gulp-2x.png" width="50px"><img src="https://wordimpress.com/assets/icon-grunt.png" width="50px"><img src="https://farm8.staticflickr.com/7255/7543242464_58d5d8ebae_z.jpg" width="50px"><img src="https://www.pubnub.com/blog/wp-content/uploads/2014/07/SOCKETIOICON.gif" width="50px"><img src="http://yeoman.io/static/yeoman-02.dc21b7fc1d.png" width="50px"><img src="http://chaijs.com/public/img/chai-logo.png" width="50px">

---

Yeoman generator for creating MEAN stack applications, using MongoDB, Express, AngularJS, and Node - lets you quickly set up a project following best practices.

Built on:
![Build Status](https://codeship.com/projects/26128390-800a-0133-c5f7-6a23b0487a18/status?branch=master)
[![npm version](https://badge.fury.io/js/generator-angular-fullstack.svg)](http://badge.fury.io/js/generator-angular-fullstack)
[![Dependency Status](https://david-dm.org/angular-fullstack/generator-angular-fullstack.svg)](https://david-dm.org/angular-fullstack/generator-angular-fullstack)
[![Dev-Dependency Status](https://david-dm.org/angular-fullstack/generator-angular-fullstack/dev-status.svg)](https://david-dm.org/angular-fullstack/generator-angular-fullstack#info=devDependencies)
[![Gitter chat](https://badges.gitter.im/DaftMonk/generator-angular-fullstack.svg)](https://gitter.im/DaftMonk/generator-angular-fullstack) 



---

## Welcome to Universal Javascript
![](https://cdn-images-1.medium.com/max/1600/1*pkA5znpcqqmIwZRXesioGA.png)
Javascript that can run both in the client (browser) and server (ie - [Node.js](https://nodejs.org/)) is here...[read more about it here](https://medium.com/@mjackson/universal-javascript-4761051b7ae9).

### FullStack Generator
This `yeoman` universal javascript application stack generator features [Angular](https://angular.io/), [Express](http://expressjs.com), [Node](https://nodejs.org/en/), [Mongo](https://www.mongodb.org/), [Socket](http://socket.io/), and more.

Here are some of the main capabilities:

* Angular best practices ([`component`](http://www.johnpapa.net/angular-growth-structure/)/[`feature`](http://www.johnpapa.net/angular-growth-structure/) folder structure)
* SASS AND LESS enabled
* [`jshint`](http://jshint.com/), [`jscsc`](http://jscs.info/), [`eslint`](http://eslint.org/) enabled for better quality code
* [Karma](https://karma-runner.github.io/) configured with [Code Coverage](https://karma-runner.github.io/0.8/config/coverage.html)
* [Protractor](http://www.protractortest.org/) E2E Angular testing
* [Browser-sync](https://www.browsersync.io/) for synchronised browser testing
* Continuous integration with [Travic CI](https://travis-ci.org/giftstarter/generator-makeme)
* [TestFairy](http://testfairy.com/) publishing for mobile testing
* [ES6](http://www.es6js.com/)/[7](https://developer.mozilla.org/en-US/docs/Web/JavaScript/New_in_JavaScript/ECMAScript_7_support_in_Mozilla) supported by using [`the babel`](https://babeljs.io/)

---

> **NOTE:**   
> This uses [generator-fullstack-deps](https://github.com/angular-fullstack/angular-fullstack-deps) to scaffold common dependencies

## Setting up
In order to get the best experience, you have to install a couple of global npm packages, like Gulp, Yemoan, and more. 

### Prerequisites

- [Git](https://git-scm.com/)
- [Node.js and npm](nodejs.org) Node ^4.2.3, npm ^2.14.7
- [Bower](bower.io) (`npm install --global bower`)
- [Gulp](http://gulpjs.com/) (`npm install --global gulp`)
- [MongoDB](https://www.mongodb.org/) - Keep a running daemon with `mongod`


### Auto install
Execute the following command:

```
$ npm install -g yo gulp bower generator-makeme
```


This will install, among others, the following packages globally:

* gulp
* yeoman
* bower
* makeme generator


#### A few things to note:

1. If you have issues (like `$ yo: command not found`) - first run `npm install -g yo` & `npm install --global gulp`
2. If you have existing project modify the name of the generator in your `.yo-rc.json` file 
3. If you need to update Node, do this:
  1. `npm cache clean -f`
  2. Install [nvm](https://github.com/creationix/nvm#install-script)
  3. `nvm install 4.2.4`
  4. `nvm alias default 4.2.4`
  5. `nvm use 4.2.4`

---

## Supported Configurations

**General**

* Build Systems: `Grunt`, `Gulp` 
* Testing: 
  * `Jasmine`
  * `Mocha + Chai + Sinon`
    * Chai assertions:
      * `Expect`
      * `Should`

**Client**

* Scripts: `Babel`, `TypeScript` (Coming Soon)
* Markup:  `HTML`, `Jade`
* Stylesheets: `CSS`, `Stylus`, `Sass`, `Less`
* Angular Routers: `ngRoute`, `ui-router`
* CSS Frameworks: `Material`, `Bootstrap`
  * Option to include `UI Bootstrap`

**Server**

* Scripts: `Babel`
* Database:
  * `None`,
  * `MongoDB`, `SQL`
    * Authentication boilerplate: `Yes`, `No`
    * oAuth integrations: `Facebook` `Twitter` `Google`
    * Socket.io integration: `Yes`, `No`

### Configuration
The generated projects can be further tweaked according to your needs by modifying project files appropriately.

An editable `.yo-rc` file is generated for helping to copy configurations across projects, and to allow you to keep track of settings.


## Project Structure

#### Base structure

    ├── client
    │   ├── app                 - All app specific components go in here
    │   ├── assets              - Custom assets: fonts, images, etc…
    │   ├── components          - Reusable components, non-specific to this app
    │
    ├── e2e                     - Protractor end to end tests
    │
    └── server
        ├── api                 - Local server api
        ├── auth                - For handling authentication with different auth strategies
        ├── components          - Reusable or app-wide components
        ├── config              - App configurations
        │   └── local.env.js    - Keep environment variables out of source control
        │   └── environment     - Configuration specific to the node environment
        └── views               - Server rendered views

#### An example client component in `client/app`

    main
    ├── main.js                 - Routes
    ├── main.controller.js      - Controller for our main route
    ├── main.controller.spec.js - Test
    ├── main.html               - View
    └── main.less               - Styles

#### An example server component in `server/api`

    thing
    ├── index.js                - Routes
    ├── thing.controller.js     - Controller for our `thing` endpoint
    ├── thing.model.js          - Database model
    ├── thing.socket.js         - Register socket events
    └── thing.spec.js           - Test

### Environment Variables

Keeping the app secrets and other sensitive information in source control isn't a good idea. To have `gulp` (or `grunt`) launch the app with specific environment variables, add them to the git ignored environment config file: `server/config/local.env.js`.

### Injection

A `gulp` task looks for new files in your `client/app` and `client/components` folder and automatically injects them in the appropriate places based on an injection block.

* `less` files into `client/app/app.less`
* `scss` files into `client/app/app.scss`
* `stylus` files into `client/app/app.styl`
* `css` files into `client/index.html`
* `js` files into `client/index.html`
* `babel` temp `js` files into `client/index.html`



## Typical workflows
These are all available in the already provided apps, or inside any new apps you build.


1. **Develop with existing code**
 - `$ gulp serve` to start the app in `watch` mode
 - Do some `coding` that is amazing
 - `$ gulp test` to run the client & server unit tests with `karma` and `mocha`
 - View changes in a ***c9*** tab or new browser tab 
     - Click the `Preview` button in the top menu
     - Or, go to https://gs-web-username.c9.io
 - `$ gulp` to build the `client` app into the **`dist`** folder
 - `$ gulp buildcontrol:heroku` to push changes to Heroku server
2. **Develop a new component (module, controller, factory, etc)**
 - `$ yo makeme:route newModuleName`
 - `$ yo makeme:controller newControllerName`
 - [?] Where would you like to create this controller? `client/app/newModuleName`
 - `$ gulp serve` to start the app in `watch` mode
 - Do some `coding` that is amazing
 - `$ gulp test` to run the client & server unit tests with `karma` and `mocha`
 - View changes in a ***c9*** tab or new browser tab 
     - Click the `Preview` button in the top menu
     - Or, go to https://gs-web-username.c9.io
 - `$ gulp` to build the `client` app into the **`dist`** folder
 - `$ gulp buildcontrol:heroku` to push changes to Heroku server



#### - To see more, check out the [Generator docs](./docs/generators.md).



## Gulp tasks
Here is a set of simple gulp tasks available:
```
gulp                # Build the app
gulp serve          # Load the app in preview mode
gulp serve:debug	# Load a more debugging-friendly environment
gulp dist           # Distribute the application
------
gulp help           # List the main gulp tasks
gulp lint           # Run lint
gulp test           # Run lint, unit tests, and e2e tests
gulp unit           # Run lint and unit tests (karma for client + mocha for server)
gulp karma          # Run karma client unit tests
gulp mocha          # Run mocha server unit tests
gulp e2e            # Run protractor for end to end tests
gulp style          # Generate a main.css file
```



## Running the server
Here are the main ways of running the app, which includes both an Express server, MongoDB server, and an Angular client app.

1. Open `server/index.js` and start the app by clicking on the `Run` button in the top menu.
2. Alternatively you can launch the app from the `Terminal`:

    - `$ gulp serve` to preview
    - `$ gulp serve:dist` to preview the built app
    - `$ gulp serve:debug` to run the app in debug mode
    - `$ node server/index` to run the production version of the app
    
Once the server is running, open the project in the shape of `https://projectname-username.c9.io:3001`

## Bower Components

The following packages are always installed by the [app](#app) generator:

* angular
* angular-cookies
* angular-mocks
* angular-resource
* angular-sanitize
* es5-shim
* font-awesome
* json3
* jquery
* lodash

These packages are installed optionally depending on your configuration:

* angular-route
* angular-ui-router
* angular-socket-io
* angular-bootstrap
* angular-material
* angular-famous
* bootstrap

All of these can be updated with `bower update` as new versions are released.

### Adding Bower packages
You should always prefer an `npm` package instead of a `bower` package. Most of client side libraries nowadays exist as both npm and bower packages. But sometimes it is not the case and you have to deal with a bower package. Here's how to do it elegantly.

To include a third party `bower` package do the following:

* `bower install --save thepackage`
* modify `package.json` `browser` section to include a path to the global minified javascript file of the package
* if the package exposes a global `.scss` file import it into `client/styles/main.scss` and ajdust eventually the variable for the path font (should be `../fonts`)
* if the package only exposes a `.css` file adjust the **css** file constants (`gulp/common/constants.js`) to include it
* if the package relies on other libraries
  * Either add a browser-shim section 
  * Or make sure to require the dependencies in the code just before you `require` the package.
  * 
## Changelog

Recent changes can be viewed on Github on the [Releases Page](https://github.com/giftstarter/makeme/releases)


## Upgrade
Here is the core generator upgrade process.

**1:**
```bash
npm update -g generator-makeme
```
**2:**
```bash
git pull github master
```
from [makeme](https://github.com/giftstarter/makeme)

## Contribute

See the [contributing docs](https://github.com/giftstarter/generator-makeme/blob/master/contributing.md)

This project has 2 main branches: `master` and `canary`. The `master` branch is where the current stable code lives and should be used for production setups. The `canary` branch is the main development branch, this is where PRs should be submitted to (backport fixes may be applied to `master`).

By separating the current stable code from the cutting-edge development we hope to provide a stable and efficient workflow for users and developers alike.

When submitting an issue, please follow the [guidelines](https://github.com/yeoman/yeoman/blob/master/contributing.md#issue-submission). Especially important is to make sure Yeoman is up-to-date, and providing the command or commands that cause the issue.

When submitting a PR, make sure that the commit messages match the [AngularJS conventions](https://docs.google.com/document/d/1QrDFcIiPjSLDn3EL15IJygNPiHORgU1_OOAqWjiDU5Y/).

When submitting a bugfix, try to write a test that exposes the bug and fails before applying your fix. Submit the test alongside the fix.

When submitting a new feature, add tests that cover the feature.

See the `travis.yml` for configuration required to run tests.

## License

[BSD license](http://opensource.org/licenses/bsd-license.php) from [angular-fullstack](https://github.com/angular-fullstack/generator-angular-fullstack/blob/master/readme.md#license)