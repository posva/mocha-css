# mocha-css

> A mocha stylesheet for the HTML reporter that let you append visual tests

[![CircleCI][circleci-image]][circleci-url] [![npm][npm-image]][npm-url] [![license][license-image]][license-url]

![mocha-css](https://cloud.githubusercontent.com/assets/664177/20640621/7cc2fa32-b3e3-11e6-8db0-f927e67a2584.png)

In the screenshot below the `h1` element doesn't have the original mocha.css
style applied.

You have to make sure to reset the `font` property on your visual test
container. eg: If you apply the class `test-dom-container` to all of them, You'll
have to add this CSS snippet:

``` css
.test-dom-container {
  font: initial;
}
```

## Installation

**NPM**

``` sh
npm install --save-dev mocha-css
```

## Usage

Simply replace the `mocha.css` file you're importing with this one

**Webpack**

``` js
// es6
import 'mocha-css'
// commonjs
require('mocha-css')
// with loader query
import 'style-loader!css-loader!mocha-css'
```

**CDN**

``` html
<link href="https://unpkg.com/mocha-css" rel="stylesheet" />
```

[license-image]: https://img.shields.io/npm/l/normalize.css.svg?style=flat-square
[license-url]: LICENSE.md
[npm-image]: https://img.shields.io/npm/v/mocha-css.svg?style=flat-square
[npm-url]: https://www.npmjs.com/package/mocha-css
[circleci-image]: https://circleci.com/gh/posva/mocha-css/tree/master.svg?style=shield
[circleci-url]: https://circleci.com/gh/posva/mocha-css

## What is visual testing?

Visual testing consists in seeing what your tests are doing. This is useful when
authoring a UI component library because you always want to check what your
component looks like.

### Resources

- [Visual TDD and awesome documentation](http://toucantoco.com/front/2016/09/14/visual-tdd.html)
