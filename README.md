# api documentation for  [core-js (v2.4.1)](https://github.com/zloirock/core-js#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-core-js.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-core-js) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-core-js.svg)](https://travis-ci.org/npmdoc/node-npmdoc-core-js)
#### Standard library

[![NPM](https://nodei.co/npm/core-js.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/core-js)

[![apidoc](https://npmdoc.github.io/node-npmdoc-core-js/build/screenCapture.buildCi.browser.apidoc.html.png)](https://npmdoc.github.io/node-npmdoc-core-js/build/apidoc.html)

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
    "version": "2.4.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module core-js](#apidoc.module.core-js)
1.  [function <span class="apidocSignatureSpan">core-js.</span>getIterator (it)](#apidoc.element.core-js.getIterator)
1.  [function <span class="apidocSignatureSpan">core-js.</span>getIteratorMethod (it)](#apidoc.element.core-js.getIteratorMethod)
1.  [function <span class="apidocSignatureSpan">core-js.</span>inspectSource (it)](#apidoc.element.core-js.inspectSource)
1.  [function <span class="apidocSignatureSpan">core-js.</span>isIterable (it)](#apidoc.element.core-js.isIterable)
1.  object <span class="apidocSignatureSpan">core-js.</span>Array
1.  object <span class="apidocSignatureSpan">core-js.</span>Array.prototype
1.  object <span class="apidocSignatureSpan">core-js.</span>Date
1.  object <span class="apidocSignatureSpan">core-js.</span>Date.prototype
1.  object <span class="apidocSignatureSpan">core-js.</span>Error
1.  object <span class="apidocSignatureSpan">core-js.</span>Function
1.  object <span class="apidocSignatureSpan">core-js.</span>Function.prototype
1.  object <span class="apidocSignatureSpan">core-js.</span>JSON
1.  object <span class="apidocSignatureSpan">core-js.</span>Math
1.  object <span class="apidocSignatureSpan">core-js.</span>Number
1.  object <span class="apidocSignatureSpan">core-js.</span>Number.prototype
1.  object <span class="apidocSignatureSpan">core-js.</span>Object
1.  object <span class="apidocSignatureSpan">core-js.</span>Reflect
1.  object <span class="apidocSignatureSpan">core-js.</span>RegExp
1.  object <span class="apidocSignatureSpan">core-js.</span>String
1.  object <span class="apidocSignatureSpan">core-js.</span>String.prototype
1.  object <span class="apidocSignatureSpan">core-js.</span>System
1.  object <span class="apidocSignatureSpan">core-js.</span>_
1.  object <span class="apidocSignatureSpan">core-js.</span>prototype
1.  string <span class="apidocSignatureSpan">core-js.</span>version

#### [module core-js.Array](#apidoc.module.core-js.Array)
1.  object <span class="apidocSignatureSpan">core-js.Array.</span>prototype

#### [module core-js.Array.prototype](#apidoc.module.core-js.Array.prototype)
1.  [function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>copyWithin ()](#apidoc.element.core-js.Array.prototype.copyWithin)
1.  [function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>entries ()](#apidoc.element.core-js.Array.prototype.entries)
1.  [function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>every ()](#apidoc.element.core-js.Array.prototype.every)
1.  [function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>fill ()](#apidoc.element.core-js.Array.prototype.fill)
1.  [function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>filter ()](#apidoc.element.core-js.Array.prototype.filter)
1.  [function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>find ()](#apidoc.element.core-js.Array.prototype.find)
1.  [function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>findIndex ()](#apidoc.element.core-js.Array.prototype.findIndex)
1.  [function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>forEach ()](#apidoc.element.core-js.Array.prototype.forEach)
1.  [function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>includes ()](#apidoc.element.core-js.Array.prototype.includes)
1.  [function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>indexOf ()](#apidoc.element.core-js.Array.prototype.indexOf)
1.  [function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>join ()](#apidoc.element.core-js.Array.prototype.join)
1.  [function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>keys ()](#apidoc.element.core-js.Array.prototype.keys)
1.  [function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>lastIndexOf ()](#apidoc.element.core-js.Array.prototype.lastIndexOf)
1.  [function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>map ()](#apidoc.element.core-js.Array.prototype.map)
1.  [function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>reduce ()](#apidoc.element.core-js.Array.prototype.reduce)
1.  [function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>reduceRight ()](#apidoc.element.core-js.Array.prototype.reduceRight)
1.  [function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>slice ()](#apidoc.element.core-js.Array.prototype.slice)
1.  [function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>some ()](#apidoc.element.core-js.Array.prototype.some)
1.  [function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>sort ()](#apidoc.element.core-js.Array.prototype.sort)
1.  [function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>values ()](#apidoc.element.core-js.Array.prototype.values)

#### [module core-js.Date](#apidoc.module.core-js.Date)
1.  object <span class="apidocSignatureSpan">core-js.Date.</span>prototype

#### [module core-js.Date.prototype](#apidoc.module.core-js.Date.prototype)
1.  [function <span class="apidocSignatureSpan">core-js.Date.prototype.</span>toISOString ()](#apidoc.element.core-js.Date.prototype.toISOString)
1.  [function <span class="apidocSignatureSpan">core-js.Date.prototype.</span>toJSON ()](#apidoc.element.core-js.Date.prototype.toJSON)

#### [module core-js.Function](#apidoc.module.core-js.Function)
1.  object <span class="apidocSignatureSpan">core-js.Function.</span>prototype

#### [module core-js.Function.prototype](#apidoc.module.core-js.Function.prototype)
1.  [function <span class="apidocSignatureSpan">core-js.Function.prototype.</span>bind ()](#apidoc.element.core-js.Function.prototype.bind)
1.  [function <span class="apidocSignatureSpan">core-js.Function.prototype.</span>part ()](#apidoc.element.core-js.Function.prototype.part)

#### [module core-js.Number](#apidoc.module.core-js.Number)
1.  object <span class="apidocSignatureSpan">core-js.Number.</span>prototype

#### [module core-js.Number.prototype](#apidoc.module.core-js.Number.prototype)
1.  [function <span class="apidocSignatureSpan">core-js.Number.prototype.</span>toFixed ()](#apidoc.element.core-js.Number.prototype.toFixed)
1.  [function <span class="apidocSignatureSpan">core-js.Number.prototype.</span>toPrecision ()](#apidoc.element.core-js.Number.prototype.toPrecision)

#### [module core-js.String](#apidoc.module.core-js.String)
1.  object <span class="apidocSignatureSpan">core-js.String.</span>prototype

#### [module core-js.String.prototype](#apidoc.module.core-js.String.prototype)
1.  [function <span class="apidocSignatureSpan">core-js.String.prototype.</span>anchor ()](#apidoc.element.core-js.String.prototype.anchor)
1.  [function <span class="apidocSignatureSpan">core-js.String.prototype.</span>at ()](#apidoc.element.core-js.String.prototype.at)
1.  [function <span class="apidocSignatureSpan">core-js.String.prototype.</span>big ()](#apidoc.element.core-js.String.prototype.big)
1.  [function <span class="apidocSignatureSpan">core-js.String.prototype.</span>blink ()](#apidoc.element.core-js.String.prototype.blink)
1.  [function <span class="apidocSignatureSpan">core-js.String.prototype.</span>bold ()](#apidoc.element.core-js.String.prototype.bold)
1.  [function <span class="apidocSignatureSpan">core-js.String.prototype.</span>codePointAt ()](#apidoc.element.core-js.String.prototype.codePointAt)
1.  [function <span class="apidocSignatureSpan">core-js.String.prototype.</span>endsWith ()](#apidoc.element.core-js.String.prototype.endsWith)
1.  [function <span class="apidocSignatureSpan">core-js.String.prototype.</span>escapeHTML ()](#apidoc.element.core-js.String.prototype.escapeHTML)
1.  [function <span class="apidocSignatureSpan">core-js.String.prototype.</span>fixed ()](#apidoc.element.core-js.String.prototype.fixed)
1.  [function <span class="apidocSignatureSpan">core-js.String.prototype.</span>fontcolor ()](#apidoc.element.core-js.String.prototype.fontcolor)
1.  [function <span class="apidocSignatureSpan">core-js.String.prototype.</span>fontsize ()](#apidoc.element.core-js.String.prototype.fontsize)
1.  [function <span class="apidocSignatureSpan">core-js.String.prototype.</span>includes ()](#apidoc.element.core-js.String.prototype.includes)
1.  [function <span class="apidocSignatureSpan">core-js.String.prototype.</span>italics ()](#apidoc.element.core-js.String.prototype.italics)
1.  [function <span class="apidocSignatureSpan">core-js.String.prototype.</span>link ()](#apidoc.element.core-js.String.prototype.link)
1.  [function <span class="apidocSignatureSpan">core-js.String.prototype.</span>matchAll ()](#apidoc.element.core-js.String.prototype.matchAll)
1.  [function <span class="apidocSignatureSpan">core-js.String.prototype.</span>padEnd ()](#apidoc.element.core-js.String.prototype.padEnd)
1.  [function <span class="apidocSignatureSpan">core-js.String.prototype.</span>padStart ()](#apidoc.element.core-js.String.prototype.padStart)
1.  [function <span class="apidocSignatureSpan">core-js.String.prototype.</span>repeat ()](#apidoc.element.core-js.String.prototype.repeat)
1.  [function <span class="apidocSignatureSpan">core-js.String.prototype.</span>small ()](#apidoc.element.core-js.String.prototype.small)
1.  [function <span class="apidocSignatureSpan">core-js.String.prototype.</span>startsWith ()](#apidoc.element.core-js.String.prototype.startsWith)
1.  [function <span class="apidocSignatureSpan">core-js.String.prototype.</span>strike ()](#apidoc.element.core-js.String.prototype.strike)
1.  [function <span class="apidocSignatureSpan">core-js.String.prototype.</span>sub ()](#apidoc.element.core-js.String.prototype.sub)
1.  [function <span class="apidocSignatureSpan">core-js.String.prototype.</span>sup ()](#apidoc.element.core-js.String.prototype.sup)
1.  [function <span class="apidocSignatureSpan">core-js.String.prototype.</span>trim ()](#apidoc.element.core-js.String.prototype.trim)
1.  [function <span class="apidocSignatureSpan">core-js.String.prototype.</span>trimEnd ()](#apidoc.element.core-js.String.prototype.trimEnd)
1.  [function <span class="apidocSignatureSpan">core-js.String.prototype.</span>trimLeft ()](#apidoc.element.core-js.String.prototype.trimLeft)
1.  [function <span class="apidocSignatureSpan">core-js.String.prototype.</span>trimRight ()](#apidoc.element.core-js.String.prototype.trimRight)
1.  [function <span class="apidocSignatureSpan">core-js.String.prototype.</span>trimStart ()](#apidoc.element.core-js.String.prototype.trimStart)
1.  [function <span class="apidocSignatureSpan">core-js.String.prototype.</span>unescapeHTML ()](#apidoc.element.core-js.String.prototype.unescapeHTML)



# <a name="apidoc.module.core-js"></a>[module core-js](#apidoc.module.core-js)

#### <a name="apidoc.element.core-js.getIterator"></a>[function <span class="apidocSignatureSpan">core-js.</span>getIterator (it)](#apidoc.element.core-js.getIterator)
- description and source-code
```javascript
getIterator = function (it){
  var iterFn = get(it);
  if(typeof iterFn != 'function')throw TypeError(it + ' is not iterable!');
  return anObject(iterFn.call(it));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.getIteratorMethod"></a>[function <span class="apidocSignatureSpan">core-js.</span>getIteratorMethod (it)](#apidoc.element.core-js.getIteratorMethod)
- description and source-code
```javascript
getIteratorMethod = function (it){
  if(it != undefined)return it[ITERATOR]
    || it['@@iterator']
    || Iterators[classof(it)];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.inspectSource"></a>[function <span class="apidocSignatureSpan">core-js.</span>inspectSource (it)](#apidoc.element.core-js.inspectSource)
- description and source-code
```javascript
inspectSource = function (it){
  return $toString.call(it);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.isIterable"></a>[function <span class="apidocSignatureSpan">core-js.</span>isIterable (it)](#apidoc.element.core-js.isIterable)
- description and source-code
```javascript
isIterable = function (it){
  var O = Object(it);
  return O[ITERATOR] !== undefined
    || '@@iterator' in O
    || Iterators.hasOwnProperty(classof(O));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.core-js.Array"></a>[module core-js.Array](#apidoc.module.core-js.Array)



# <a name="apidoc.module.core-js.Array.prototype"></a>[module core-js.Array.prototype](#apidoc.module.core-js.Array.prototype)

#### <a name="apidoc.element.core-js.Array.prototype.copyWithin"></a>[function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>copyWithin ()](#apidoc.element.core-js.Array.prototype.copyWithin)
- description and source-code
```javascript
function copyWithin() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.Array.prototype.entries"></a>[function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>entries ()](#apidoc.element.core-js.Array.prototype.entries)
- description and source-code
```javascript
function entries() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.Array.prototype.every"></a>[function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>every ()](#apidoc.element.core-js.Array.prototype.every)
- description and source-code
```javascript
function every() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.Array.prototype.fill"></a>[function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>fill ()](#apidoc.element.core-js.Array.prototype.fill)
- description and source-code
```javascript
function fill() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.Array.prototype.filter"></a>[function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>filter ()](#apidoc.element.core-js.Array.prototype.filter)
- description and source-code
```javascript
function filter() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.Array.prototype.find"></a>[function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>find ()](#apidoc.element.core-js.Array.prototype.find)
- description and source-code
```javascript
function find() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.Array.prototype.findIndex"></a>[function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>findIndex ()](#apidoc.element.core-js.Array.prototype.findIndex)
- description and source-code
```javascript
function findIndex() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.Array.prototype.forEach"></a>[function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>forEach ()](#apidoc.element.core-js.Array.prototype.forEach)
- description and source-code
```javascript
function forEach() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.Array.prototype.includes"></a>[function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>includes ()](#apidoc.element.core-js.Array.prototype.includes)
- description and source-code
```javascript
function includes() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.Array.prototype.indexOf"></a>[function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>indexOf ()](#apidoc.element.core-js.Array.prototype.indexOf)
- description and source-code
```javascript
function indexOf() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.Array.prototype.join"></a>[function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>join ()](#apidoc.element.core-js.Array.prototype.join)
- description and source-code
```javascript
function join() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.Array.prototype.keys"></a>[function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>keys ()](#apidoc.element.core-js.Array.prototype.keys)
- description and source-code
```javascript
function keys() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.Array.prototype.lastIndexOf"></a>[function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>lastIndexOf ()](#apidoc.element.core-js.Array.prototype.lastIndexOf)
- description and source-code
```javascript
function lastIndexOf() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.Array.prototype.map"></a>[function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>map ()](#apidoc.element.core-js.Array.prototype.map)
- description and source-code
```javascript
function map() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.Array.prototype.reduce"></a>[function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>reduce ()](#apidoc.element.core-js.Array.prototype.reduce)
- description and source-code
```javascript
function reduce() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.Array.prototype.reduceRight"></a>[function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>reduceRight ()](#apidoc.element.core-js.Array.prototype.reduceRight)
- description and source-code
```javascript
function reduceRight() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.Array.prototype.slice"></a>[function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>slice ()](#apidoc.element.core-js.Array.prototype.slice)
- description and source-code
```javascript
function slice() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.Array.prototype.some"></a>[function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>some ()](#apidoc.element.core-js.Array.prototype.some)
- description and source-code
```javascript
function some() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.Array.prototype.sort"></a>[function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>sort ()](#apidoc.element.core-js.Array.prototype.sort)
- description and source-code
```javascript
function sort() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.Array.prototype.values"></a>[function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>values ()](#apidoc.element.core-js.Array.prototype.values)
- description and source-code
```javascript
function values() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.core-js.Date"></a>[module core-js.Date](#apidoc.module.core-js.Date)



# <a name="apidoc.module.core-js.Date.prototype"></a>[module core-js.Date.prototype](#apidoc.module.core-js.Date.prototype)

#### <a name="apidoc.element.core-js.Date.prototype.toISOString"></a>[function <span class="apidocSignatureSpan">core-js.Date.prototype.</span>toISOString ()](#apidoc.element.core-js.Date.prototype.toISOString)
- description and source-code
```javascript
function toISOString() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.Date.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">core-js.Date.prototype.</span>toJSON ()](#apidoc.element.core-js.Date.prototype.toJSON)
- description and source-code
```javascript
function toJSON() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.core-js.Function"></a>[module core-js.Function](#apidoc.module.core-js.Function)



# <a name="apidoc.module.core-js.Function.prototype"></a>[module core-js.Function.prototype](#apidoc.module.core-js.Function.prototype)

#### <a name="apidoc.element.core-js.Function.prototype.bind"></a>[function <span class="apidocSignatureSpan">core-js.Function.prototype.</span>bind ()](#apidoc.element.core-js.Function.prototype.bind)
- description and source-code
```javascript
function bind() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.Function.prototype.part"></a>[function <span class="apidocSignatureSpan">core-js.Function.prototype.</span>part ()](#apidoc.element.core-js.Function.prototype.part)
- description and source-code
```javascript
function part() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.core-js.Number"></a>[module core-js.Number](#apidoc.module.core-js.Number)



# <a name="apidoc.module.core-js.Number.prototype"></a>[module core-js.Number.prototype](#apidoc.module.core-js.Number.prototype)

#### <a name="apidoc.element.core-js.Number.prototype.toFixed"></a>[function <span class="apidocSignatureSpan">core-js.Number.prototype.</span>toFixed ()](#apidoc.element.core-js.Number.prototype.toFixed)
- description and source-code
```javascript
function toFixed() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.Number.prototype.toPrecision"></a>[function <span class="apidocSignatureSpan">core-js.Number.prototype.</span>toPrecision ()](#apidoc.element.core-js.Number.prototype.toPrecision)
- description and source-code
```javascript
function toPrecision() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.core-js.String"></a>[module core-js.String](#apidoc.module.core-js.String)



# <a name="apidoc.module.core-js.String.prototype"></a>[module core-js.String.prototype](#apidoc.module.core-js.String.prototype)

#### <a name="apidoc.element.core-js.String.prototype.anchor"></a>[function <span class="apidocSignatureSpan">core-js.String.prototype.</span>anchor ()](#apidoc.element.core-js.String.prototype.anchor)
- description and source-code
```javascript
function anchor() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.String.prototype.at"></a>[function <span class="apidocSignatureSpan">core-js.String.prototype.</span>at ()](#apidoc.element.core-js.String.prototype.at)
- description and source-code
```javascript
function at() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.String.prototype.big"></a>[function <span class="apidocSignatureSpan">core-js.String.prototype.</span>big ()](#apidoc.element.core-js.String.prototype.big)
- description and source-code
```javascript
function big() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.String.prototype.blink"></a>[function <span class="apidocSignatureSpan">core-js.String.prototype.</span>blink ()](#apidoc.element.core-js.String.prototype.blink)
- description and source-code
```javascript
function blink() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.String.prototype.bold"></a>[function <span class="apidocSignatureSpan">core-js.String.prototype.</span>bold ()](#apidoc.element.core-js.String.prototype.bold)
- description and source-code
```javascript
function bold() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.String.prototype.codePointAt"></a>[function <span class="apidocSignatureSpan">core-js.String.prototype.</span>codePointAt ()](#apidoc.element.core-js.String.prototype.codePointAt)
- description and source-code
```javascript
function codePointAt() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.String.prototype.endsWith"></a>[function <span class="apidocSignatureSpan">core-js.String.prototype.</span>endsWith ()](#apidoc.element.core-js.String.prototype.endsWith)
- description and source-code
```javascript
function endsWith() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.String.prototype.escapeHTML"></a>[function <span class="apidocSignatureSpan">core-js.String.prototype.</span>escapeHTML ()](#apidoc.element.core-js.String.prototype.escapeHTML)
- description and source-code
```javascript
function escapeHTML() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.String.prototype.fixed"></a>[function <span class="apidocSignatureSpan">core-js.String.prototype.</span>fixed ()](#apidoc.element.core-js.String.prototype.fixed)
- description and source-code
```javascript
function fixed() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.String.prototype.fontcolor"></a>[function <span class="apidocSignatureSpan">core-js.String.prototype.</span>fontcolor ()](#apidoc.element.core-js.String.prototype.fontcolor)
- description and source-code
```javascript
function fontcolor() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.String.prototype.fontsize"></a>[function <span class="apidocSignatureSpan">core-js.String.prototype.</span>fontsize ()](#apidoc.element.core-js.String.prototype.fontsize)
- description and source-code
```javascript
function fontsize() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.String.prototype.includes"></a>[function <span class="apidocSignatureSpan">core-js.String.prototype.</span>includes ()](#apidoc.element.core-js.String.prototype.includes)
- description and source-code
```javascript
function includes() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.String.prototype.italics"></a>[function <span class="apidocSignatureSpan">core-js.String.prototype.</span>italics ()](#apidoc.element.core-js.String.prototype.italics)
- description and source-code
```javascript
function italics() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.String.prototype.link"></a>[function <span class="apidocSignatureSpan">core-js.String.prototype.</span>link ()](#apidoc.element.core-js.String.prototype.link)
- description and source-code
```javascript
function link() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.String.prototype.matchAll"></a>[function <span class="apidocSignatureSpan">core-js.String.prototype.</span>matchAll ()](#apidoc.element.core-js.String.prototype.matchAll)
- description and source-code
```javascript
function matchAll() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.String.prototype.padEnd"></a>[function <span class="apidocSignatureSpan">core-js.String.prototype.</span>padEnd ()](#apidoc.element.core-js.String.prototype.padEnd)
- description and source-code
```javascript
function padEnd() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.String.prototype.padStart"></a>[function <span class="apidocSignatureSpan">core-js.String.prototype.</span>padStart ()](#apidoc.element.core-js.String.prototype.padStart)
- description and source-code
```javascript
function padStart() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.String.prototype.repeat"></a>[function <span class="apidocSignatureSpan">core-js.String.prototype.</span>repeat ()](#apidoc.element.core-js.String.prototype.repeat)
- description and source-code
```javascript
function repeat() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.String.prototype.small"></a>[function <span class="apidocSignatureSpan">core-js.String.prototype.</span>small ()](#apidoc.element.core-js.String.prototype.small)
- description and source-code
```javascript
function small() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.String.prototype.startsWith"></a>[function <span class="apidocSignatureSpan">core-js.String.prototype.</span>startsWith ()](#apidoc.element.core-js.String.prototype.startsWith)
- description and source-code
```javascript
function startsWith() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.String.prototype.strike"></a>[function <span class="apidocSignatureSpan">core-js.String.prototype.</span>strike ()](#apidoc.element.core-js.String.prototype.strike)
- description and source-code
```javascript
function strike() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.String.prototype.sub"></a>[function <span class="apidocSignatureSpan">core-js.String.prototype.</span>sub ()](#apidoc.element.core-js.String.prototype.sub)
- description and source-code
```javascript
function sub() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.String.prototype.sup"></a>[function <span class="apidocSignatureSpan">core-js.String.prototype.</span>sup ()](#apidoc.element.core-js.String.prototype.sup)
- description and source-code
```javascript
function sup() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.String.prototype.trim"></a>[function <span class="apidocSignatureSpan">core-js.String.prototype.</span>trim ()](#apidoc.element.core-js.String.prototype.trim)
- description and source-code
```javascript
function trim() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.String.prototype.trimEnd"></a>[function <span class="apidocSignatureSpan">core-js.String.prototype.</span>trimEnd ()](#apidoc.element.core-js.String.prototype.trimEnd)
- description and source-code
```javascript
function trimEnd() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.String.prototype.trimLeft"></a>[function <span class="apidocSignatureSpan">core-js.String.prototype.</span>trimLeft ()](#apidoc.element.core-js.String.prototype.trimLeft)
- description and source-code
```javascript
function trimStart() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.String.prototype.trimRight"></a>[function <span class="apidocSignatureSpan">core-js.String.prototype.</span>trimRight ()](#apidoc.element.core-js.String.prototype.trimRight)
- description and source-code
```javascript
function trimEnd() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.String.prototype.trimStart"></a>[function <span class="apidocSignatureSpan">core-js.String.prototype.</span>trimStart ()](#apidoc.element.core-js.String.prototype.trimStart)
- description and source-code
```javascript
function trimStart() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.String.prototype.unescapeHTML"></a>[function <span class="apidocSignatureSpan">core-js.String.prototype.</span>unescapeHTML ()](#apidoc.element.core-js.String.prototype.unescapeHTML)
- description and source-code
```javascript
function unescapeHTML() { [native code] }
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
