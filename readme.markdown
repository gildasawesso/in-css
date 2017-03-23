# insert-css

[![npm](https://img.shields.io/badge/npm-3.10.10-blue.svg)]()
[![npm version](https://badge.fury.io/js/insert-css.svg)](https://badge.fury.io/js/insert-css)
[![dependencies](https://david-dm.org/GhaniaH/insert-css.svg)]()
[![dev dependencies](https://img.shields.io/david/dev/GhaniaH/insert-css.svg)]()
[![Coveralls](https://img.shields.io/coveralls/GhaniaH/insert-css.svg)]()
[![coverage](https://codecov.io/gh/GhaniaH/insert-css/branch/master/graph/badge.svg)](https://codecov.io/gh/GhaniaH/insert-css)
[![codecov](https://codecov.io/gh/gildasawesso/in-css/branch/master/graph/badge.svg)](https://codecov.io/gh/gildasawesso/in-css)

insert a string of css into the `<head>`

[![browser support](https://ci.testling.com/substack/insert-css.png)](https://ci.testling.com/substack/insert-css)

# example

``` js
    var insertCss = require('insert-css');
    var styleElement = insertCss('body { background:blue; }');
```

# api

``` js
    var insertCss = require('insert-css');
```

## var styleElement = insertCss(css, opts);

Insert some CSS into the page.

* `opts.container` - Which HTMLElement to use as the base mounting point, defaults to
`document.querySelector('head')`.

* `opts.prepend` - Add the CSS at the top level of the container instead of at the bottom level (default).

This is particullary useful for library creators where you may want your default CSS to be prepended so it
can be easily overriden by user styles.

# development

## example

``` sh
npm run example
```

## test

``` sh
npm test
```
