# npmdoc-core-js

#### api documentation for  [core-js (v2.4.1)](https://github.com/zloirock/core-js#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-core-js.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-core-js) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-core-js.svg)](https://travis-ci.org/npmdoc/node-npmdoc-core-js)

#### Standard library

[![NPM](https://nodei.co/npm/core-js.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/core-js)

- [https://npmdoc.github.io/node-npmdoc-core-js/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-core-js/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-core-js/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-core-js/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-core-js/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-core-js/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "bugs": {
        "url": "https://github.com/zloirock/core-js/issues"
    },
    "dependencies": {},
    "description": "Standard library",
    "devDependencies": {
        "LiveScript": "1.3.x",
        "es-observable-tests": "0.2.x",
        "eslint": "3.1.x",
        "grunt": "1.0.x",
        "grunt-cli": "1.2.x",
        "grunt-contrib-clean": "1.0.x",
        "grunt-contrib-copy": "1.0.x",
        "grunt-contrib-uglify": "1.0.x",
        "grunt-contrib-watch": "1.0.x",
        "grunt-karma": "2.0.x",
        "grunt-livescript": "0.6.x",
        "karma": "1.1.x",
        "karma-chrome-launcher": "1.0.x",
        "karma-firefox-launcher": "1.0.x",
        "karma-ie-launcher": "1.0.x",
        "karma-phantomjs-launcher": "1.0.x",
        "karma-qunit": "1.1.x",
        "phantomjs-prebuilt": "2.1.x",
        "promises-aplus-tests": "2.1.x",
        "qunitjs": "2.0.x",
        "temp": "0.8.x",
        "webpack": "1.13.x"
    },
    "directories": {},
    "dist": {
        "shasum": "4de911e667b0eae9124e34254b53aea6fc618d3e",
        "tarball": "https://registry.npmjs.org/core-js/-/core-js-2.4.1.tgz"
    },
    "gitHead": "5e106f64c726edf2849f0babc9096ce6664b7368",
    "homepage": "https://github.com/zloirock/core-js#readme",
    "keywords": [
        "ES3",
        "ECMAScript 3",
        "ES5",
        "ECMAScript 5",
        "ES6",
        "ES2015",
        "ECMAScript 6",
        "ECMAScript 2015",
        "ES7",
        "ES2016",
        "ECMAScript 7",
        "ECMAScript 2016",
        "Harmony",
        "Strawman",
        "Map",
        "Set",
        "WeakMap",
        "WeakSet",
        "Promise",
        "Symbol",
        "TypedArray",
        "setImmediate",
        "Dict",
        "polyfill",
        "shim"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "zloirock"
        }
    ],
    "name": "core-js",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/zloirock/core-js.git"
    },
    "scripts": {
        "grunt": "grunt",
        "lint": "eslint es5 es6 es7 stage web core fn modules",
        "observables-tests": "node tests/observables/adapter && node tests/observables/adapter-library",
        "promises-tests": "promises-aplus-tests tests/promises-aplus/adapter",
        "test": "npm run lint && npm run grunt livescript client karma:default && npm run grunt library karma:library && npm run promises-tests && npm run observables-tests && lsc tests/commonjs"
    },
    "version": "2.4.1",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
