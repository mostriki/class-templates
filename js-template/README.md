# Javascript Track Project Setup
___
### Project Files
`touch index.html .gitignore README.md gulpfile.js js/NAME_OF_PROJECT.js js/NAME_OF_PROJECT-INTERFACE.js`

##### index.html header
```
<head>
  <link rel="stylesheet" href="build/css/vendor.css">
  <link href="build/css/vendor.css" rel="stylesheet" type="text/css">
  <script src="build/js/vendor.min.js"></script>
  <script type="text/javascript" src="build/js/app.js"></script>
</head>
```
___
## npm
_If you don't want to fuss with installing each package individually, just copy and paste the package.json, gulpfile.js, and karma.conf.js files, then `npm install`._

_OR_

1. `npm init`
1. `npm install gulp --save-dev` (global install: `npm install gulp -g`)
1. `npm install bower -g`
1. `npm install browserify --save-dev`
1. `npm install vinyl-source-stream --save-dev`
1. `npm install gulp-concat --save-dev`
1. `npm install gulp-uglify --save-dev`
1. `npm install gulp-util --save-dev`
1. `npm install del --save-dev`
1. `npm install jshint --save-dev`
1. `npm install gulp-jshint --save-dev`
1. `npm install bower-files --save-dev`
1. `npm install browser-sync --save-dev`
1. `npm install watchify --save-dev`
1. `npm install jasmine --save-dev`
1. `npm install karma --save-dev`
1. `npm install karma-jasmine jasmine-core --save-dev`
1. `npm install karma-chrome-launcher --save-dev`
1. `npm install karma-cli --save-dev`
1. `npm install karma-browserify --save-dev`
1. `npm install karma-jquery --save-dev`
1. `npm install karma-jasmine-html-reporter --save-dev`
1. `npm install babelify babel-preset-es2015 --save-dev`

#### OR...Master npm Setup Command (Must run `npm init` first)
_`npm install gulp bower browserify vinyl-source-stream gulp-concat gulp-uglify gulp-util del jshint gulp-jshint bower-files browser-sync watchify jasmine karma karma-jasmine jasmine-core karma-chrome-launcher karma-cli karma-browserify karma-jquery karma-jasmine-html-reporter babelify babel-preset-es2015 --save-dev`_
___
### bower
* `bower init`
* `bower install jquery --save`
* `bower install bootstrap#v4.0.0-beta --save`
* `bower install moment --save`

#### OR...Master npm Setup Command (Must run `bower init` first)
_`bower install jquery bootstrap#v4.0.0-beta moment --save`_
___
### Jasmine (Install before Karma)
* ` ./node_modules/.bin/jasmine init`
_Make sure to include the below "scripts" in the package.json file._

```
...
"scripts": {
  "test": "jasmine"
}
...
```
___
### Karma
_Use provided template "karma.conf.js" instead._

_OR_

_`karma init` in root proj directory_
___
### gulp stuff
* Make sure the backend js has corresponding exports at the bottom of the file (ex. `exports.module_NameModule = Module_Name;`)
* Make sure the frontend js has corresponding requires at the top of the file (ex. `var ComputerPlayer = require('./../js/pig.js').computerPlayerModule;`)
* Run `gulp build` before you fire up the browser.
___
### jshint (ES6)
_configure jshint for ES6 by creating a .jshintrc file in the root directory._

`{ "esversion":6 }`
___
# Javascript Track Project Clone

* `npm init`
* `npm install`
* `npm install bower -g`
* `bower init`
* `bower install`
* `gulp build`
___
# BrowserSync
_Install a package called BrowserSync to implement our development server with live reloading._

`gulp serve`
