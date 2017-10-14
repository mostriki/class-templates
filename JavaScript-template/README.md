# **INSTALLATION CHECKLIST**

#### A helpful template for getting started each day, 08.02.2017

## _By and for the fall/winter Ruby Class at Epicodus_

### Initial files you should make

* css
  * styles.css
* js
  * [NAME-OF-PROJECT].js 6
  * [NAME-OF-PROJECT]-interface.js
* spec
  * [NAME-OF-PROJECT]-spec.js
* .gitignore
* .jshintrc
* gulpfile.js
* index.html
* README.md


```
<head>
  <link rel="stylesheet" href="build/css/vendor.css">
  <link href="build/css/vendor.css" rel="stylesheet" type="text/css">
  <script src="build/js/vendor.min.js"></script>
  <script type="text/javascript" src="build/js/app.js"></script>
</head>
```
___
### Installation Option 1 (recommended)

* `$ git init`
* `git remote add [INITIALS] [GitHub Rep]`
* Copy and paste gulpfile.js
* Copy and paste package.json
* Copy and paste karma.conf.js
* `$ npm install` in your root project directory.

* `bower init`
* `bower install jquery --save`
* `bower install bootstrap#v4.0.0-beta --save`
* `bower install moment --save`
___
### Installation Option 2

* `$ git init`
* `git remote add [INITIALS] [GitHub Rep]`
* `npm init`
* `npm install gulp --save-dev`
* `npm install bower -g`
* `npm install browserify --save-dev`
* `npm install vinyl-source-stream --save-dev`
* `npm install gulp-concat --save-dev`
* `npm install gulp-uglify --save-dev`
* `npm install gulp-util --save-dev`
* `npm install del --save-dev`
* `npm install jshint --save-dev`
* `npm install gulp-jshint --save-dev`
* `npm install bower-files --save-dev`
* `npm install browser-sync --save-dev`
* `npm install watchify --save-dev`
* `npm install jasmine --save-dev`
* `npm install karma --save-dev`
* `npm install karma-jasmine jasmine-core --save-dev`
* `npm install karma-chrome-launcher --save-dev`
* `npm install karma-cli --save-dev`
* `npm install karma-browserify --save-dev`
* `npm install karma-jquery --save-dev`
* `npm install karma-jasmine-html-reporter --save-dev`
* `npm install babelify babel-preset-es2015 --save-dev`

* `bower init`
* `bower install jquery --save`
* `bower install bootstrap#v4.0.0-beta --save`
* `bower install moment --save`
___
### Installation Option 3

* `$ git init`
* `git remote add [INITIALS] [GitHub Rep]`
* `npm init`

_`npm install gulp bower browserify vinyl-source-stream gulp-concat gulp-uglify gulp-util del jshint gulp-jshint bower-files browser-sync watchify jasmine karma karma-jasmine jasmine-core karma-chrome-launcher karma-cli karma-browserify karma-jquery karma-jasmine-html-reporter babelify babel-preset-es2015 --save-dev`_

_`bower install jquery bootstrap#v4.0.0-beta moment --save`_
___
### When cloning from your GitHub Repo

* `npm install`
* `bower install`
* `gulp build`
___
# BrowserSync

* `gulp serve` to run on a local server.
___
### Optional

* OPTIONAL: globaly install gulp if you need to: `npm install gulp -g`
* OPTIONAL: globaly install bower if you need to: `npm install bower -g`


___
___
___

Things to delete once I confirm that the flow works:

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
### Karma
_Use provided template "karma.conf.js" instead._

_OR_

_`karma init` in root proj directory_
