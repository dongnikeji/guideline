<img src="https://raw.githubusercontent.com/voodootikigod/logo.js/master/js.png" width="80"
height="80" />

## Overview
* [Style Guide](#style-guide)
* [Linters](#linters)
* [Reference](#reference)

## Style Guide
It is highly recommended to read the [JavaScript style guide](https://github.com/airbnb/javascript) written by airbnb dev team. It is well-documented and should give you the basic idea on to write a nice and clean javascript for both ES5 and ES6 versions.

## Linters
A good linter can help us to identify different types of coding errors such as potential
programmatic and stylistic errors.

- [JSHint](http://jshint.com/)
    * Run `npm install -g jshint` if you want to use its cli tool;
    * Run `npm install --save-dev jshint` to install `jshint` as a dev dependency and use it locally;
    * Add a `.jshintrc` file to project directory for custom rules; There is sample `.jshint` inside this folder;
    * If you are using `sublime text` as the code editor, you may want to look at the [SublimeLinter-jshint](https://github.com/SublimeLinter/SublimeLinter-jshint) package for real-time background linting;

- [ESLint](http://eslint.org/)
    * Run `npm install -g eslint` if you want to use the cli tool;
    * Run `npm install --save-dev eslint` to use `eslint` locally;
    * Add a `.eslintrc` file to project directory for custom rules;
    * Lots of `eslint` config set can be found in the internet; You are highly recommended to look at those offered by [Airbnb][airbnb-eslint] and [Walmart Labs][watmartlabs-eslint]; You can install those rules as dev dependencies and call them by adding an `extends` entry in the project-level `.eslintrc` file;
    * For `sublime text` users, you may want to look at [SublimeLinter-contrib-eslint](https://github.com/roadhump/SublimeLinter-eslint) for background linting;

## Reference
[Rangle.io JavaScript Development Guidelines](http://rangle.io/guidelines/)

[airbnb-eslint]: https://github.com/airbnb/javascript/blob/master/packages/eslint-config-airbnb/index.js
[watmartlabs-eslint]: https://github.com/walmartlabs/eslint-config-defaults
