# api documentation for  [core-js (v2.4.1)](https://github.com/zloirock/core-js#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-core-js.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-core-js) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-core-js.svg)](https://travis-ci.org/npmdoc/node-npmdoc-core-js)
#### Standard library

[![NPM](https://nodei.co/npm/core-js.png?downloads=true)](https://www.npmjs.com/package/core-js)

[![apidoc](https://npmdoc.github.io/node-npmdoc-core-js/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-core-js_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-core-js/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-core-js/build/screen-capture.npmPackageListing.svg)



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
            "name": "zloirock",
            "email": "zloirock@zloirock.ru"
        }
    ],
    "name": "core-js",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
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
1.  [function <span class="apidocSignatureSpan">core-js.</span>_string_trim (KEY, exec, ALIAS)](#apidoc.element.core-js._string_trim)
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
1.  object <span class="apidocSignatureSpan">core-js.</span>_collection_strong
1.  object <span class="apidocSignatureSpan">core-js.</span>_collection_weak
1.  object <span class="apidocSignatureSpan">core-js.</span>_iterators
1.  object <span class="apidocSignatureSpan">core-js.</span>_meta
1.  object <span class="apidocSignatureSpan">core-js.</span>_metadata
1.  object <span class="apidocSignatureSpan">core-js.</span>_object_dp
1.  object <span class="apidocSignatureSpan">core-js.</span>_object_gopd
1.  object <span class="apidocSignatureSpan">core-js.</span>_object_gopn
1.  object <span class="apidocSignatureSpan">core-js.</span>_object_gopn_ext
1.  object <span class="apidocSignatureSpan">core-js.</span>_object_gops
1.  object <span class="apidocSignatureSpan">core-js.</span>_object_pie
1.  object <span class="apidocSignatureSpan">core-js.</span>_set_proto
1.  object <span class="apidocSignatureSpan">core-js.</span>_task
1.  object <span class="apidocSignatureSpan">core-js.</span>_typed_buffer
1.  object <span class="apidocSignatureSpan">core-js.</span>_wks_ext
1.  object <span class="apidocSignatureSpan">core-js.</span>core
1.  object <span class="apidocSignatureSpan">core-js.</span>es6_array_iterator
1.  object <span class="apidocSignatureSpan">core-js.</span>library
1.  object <span class="apidocSignatureSpan">core-js.</span>prototype
1.  object <span class="apidocSignatureSpan">core-js.</span>shim
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

#### [module core-js._collection_strong](#apidoc.module.core-js._collection_strong)
1.  [function <span class="apidocSignatureSpan">core-js._collection_strong.</span>def (that, key, value)](#apidoc.element.core-js._collection_strong.def)
1.  [function <span class="apidocSignatureSpan">core-js._collection_strong.</span>getConstructor (wrapper, NAME, IS_MAP, ADDER)](#apidoc.element.core-js._collection_strong.getConstructor)
1.  [function <span class="apidocSignatureSpan">core-js._collection_strong.</span>getEntry (that, key)](#apidoc.element.core-js._collection_strong.getEntry)
1.  [function <span class="apidocSignatureSpan">core-js._collection_strong.</span>setStrong (C, NAME, IS_MAP)](#apidoc.element.core-js._collection_strong.setStrong)

#### [module core-js._collection_weak](#apidoc.module.core-js._collection_weak)
1.  [function <span class="apidocSignatureSpan">core-js._collection_weak.</span>def (that, key, value)](#apidoc.element.core-js._collection_weak.def)
1.  [function <span class="apidocSignatureSpan">core-js._collection_weak.</span>getConstructor (wrapper, NAME, IS_MAP, ADDER)](#apidoc.element.core-js._collection_weak.getConstructor)
1.  [function <span class="apidocSignatureSpan">core-js._collection_weak.</span>ufstore (that)](#apidoc.element.core-js._collection_weak.ufstore)

#### [module core-js._iterators](#apidoc.module.core-js._iterators)
1.  [function <span class="apidocSignatureSpan">core-js._iterators.</span>Arguments ()](#apidoc.element.core-js._iterators.Arguments)
1.  [function <span class="apidocSignatureSpan">core-js._iterators.</span>Array ()](#apidoc.element.core-js._iterators.Array)
1.  [function <span class="apidocSignatureSpan">core-js._iterators.</span>Float32Array ()](#apidoc.element.core-js._iterators.Float32Array)
1.  [function <span class="apidocSignatureSpan">core-js._iterators.</span>Float64Array ()](#apidoc.element.core-js._iterators.Float64Array)
1.  [function <span class="apidocSignatureSpan">core-js._iterators.</span>Int16Array ()](#apidoc.element.core-js._iterators.Int16Array)
1.  [function <span class="apidocSignatureSpan">core-js._iterators.</span>Int32Array ()](#apidoc.element.core-js._iterators.Int32Array)
1.  [function <span class="apidocSignatureSpan">core-js._iterators.</span>Int8Array ()](#apidoc.element.core-js._iterators.Int8Array)
1.  [function <span class="apidocSignatureSpan">core-js._iterators.</span>Map ()](#apidoc.element.core-js._iterators.Map)
1.  [function <span class="apidocSignatureSpan">core-js._iterators.</span>Number ()](#apidoc.element.core-js._iterators.Number)
1.  [function <span class="apidocSignatureSpan">core-js._iterators.</span>Set ()](#apidoc.element.core-js._iterators.Set)
1.  [function <span class="apidocSignatureSpan">core-js._iterators.</span>String ()](#apidoc.element.core-js._iterators.String)
1.  [function <span class="apidocSignatureSpan">core-js._iterators.</span>Uint16Array ()](#apidoc.element.core-js._iterators.Uint16Array)
1.  [function <span class="apidocSignatureSpan">core-js._iterators.</span>Uint32Array ()](#apidoc.element.core-js._iterators.Uint32Array)
1.  [function <span class="apidocSignatureSpan">core-js._iterators.</span>Uint8Array ()](#apidoc.element.core-js._iterators.Uint8Array)
1.  [function <span class="apidocSignatureSpan">core-js._iterators.</span>Uint8ClampedArray ()](#apidoc.element.core-js._iterators.Uint8ClampedArray)

#### [module core-js._meta](#apidoc.module.core-js._meta)
1.  boolean <span class="apidocSignatureSpan">core-js._meta.</span>NEED
1.  [function <span class="apidocSignatureSpan">core-js._meta.</span>fastKey (it, create)](#apidoc.element.core-js._meta.fastKey)
1.  [function <span class="apidocSignatureSpan">core-js._meta.</span>getWeak (it, create)](#apidoc.element.core-js._meta.getWeak)
1.  [function <span class="apidocSignatureSpan">core-js._meta.</span>onFreeze (it)](#apidoc.element.core-js._meta.onFreeze)
1.  string <span class="apidocSignatureSpan">core-js._meta.</span>KEY

#### [module core-js._metadata](#apidoc.module.core-js._metadata)
1.  [function <span class="apidocSignatureSpan">core-js._metadata.</span>exp (O)](#apidoc.element.core-js._metadata.exp)
1.  [function <span class="apidocSignatureSpan">core-js._metadata.</span>get (MetadataKey, O, P)](#apidoc.element.core-js._metadata.get)
1.  [function <span class="apidocSignatureSpan">core-js._metadata.</span>has (MetadataKey, O, P)](#apidoc.element.core-js._metadata.has)
1.  [function <span class="apidocSignatureSpan">core-js._metadata.</span>key (it)](#apidoc.element.core-js._metadata.key)
1.  [function <span class="apidocSignatureSpan">core-js._metadata.</span>keys (target, targetKey)](#apidoc.element.core-js._metadata.keys)
1.  [function <span class="apidocSignatureSpan">core-js._metadata.</span>map (target, targetKey, create)](#apidoc.element.core-js._metadata.map)
1.  [function <span class="apidocSignatureSpan">core-js._metadata.</span>set (MetadataKey, MetadataValue, O, P)](#apidoc.element.core-js._metadata.set)
1.  object <span class="apidocSignatureSpan">core-js._metadata.</span>store

#### [module core-js._object_dp](#apidoc.module.core-js._object_dp)
1.  [function <span class="apidocSignatureSpan">core-js._object_dp.</span>f ()](#apidoc.element.core-js._object_dp.f)

#### [module core-js._object_gopd](#apidoc.module.core-js._object_gopd)
1.  [function <span class="apidocSignatureSpan">core-js._object_gopd.</span>f ()](#apidoc.element.core-js._object_gopd.f)

#### [module core-js._object_gopn](#apidoc.module.core-js._object_gopn)
1.  [function <span class="apidocSignatureSpan">core-js._object_gopn.</span>f ()](#apidoc.element.core-js._object_gopn.f)

#### [module core-js._object_gopn_ext](#apidoc.module.core-js._object_gopn_ext)
1.  [function <span class="apidocSignatureSpan">core-js._object_gopn_ext.</span>f (it)](#apidoc.element.core-js._object_gopn_ext.f)

#### [module core-js._object_gops](#apidoc.module.core-js._object_gops)
1.  [function <span class="apidocSignatureSpan">core-js._object_gops.</span>f ()](#apidoc.element.core-js._object_gops.f)

#### [module core-js._object_pie](#apidoc.module.core-js._object_pie)
1.  [function <span class="apidocSignatureSpan">core-js._object_pie.</span>f ()](#apidoc.element.core-js._object_pie.f)

#### [module core-js._set_proto](#apidoc.module.core-js._set_proto)
1.  [function <span class="apidocSignatureSpan">core-js._set_proto.</span>check (O, proto)](#apidoc.element.core-js._set_proto.check)
1.  [function <span class="apidocSignatureSpan">core-js._set_proto.</span>set ()](#apidoc.element.core-js._set_proto.set)

#### [module core-js._string_trim](#apidoc.module.core-js._string_trim)
1.  [function <span class="apidocSignatureSpan">core-js.</span>_string_trim (KEY, exec, ALIAS)](#apidoc.element.core-js._string_trim._string_trim)
1.  [function <span class="apidocSignatureSpan">core-js._string_trim.</span>trim (string, TYPE)](#apidoc.element.core-js._string_trim.trim)

#### [module core-js._task](#apidoc.module.core-js._task)
1.  [function <span class="apidocSignatureSpan">core-js._task.</span>clear (immediate)](#apidoc.element.core-js._task.clear)
1.  [function <span class="apidocSignatureSpan">core-js._task.</span>set (callback, arg1, arg2, arg3)](#apidoc.element.core-js._task.set)

#### [module core-js._typed_buffer](#apidoc.module.core-js._typed_buffer)
1.  [function <span class="apidocSignatureSpan">core-js._typed_buffer.</span>ArrayBuffer ()](#apidoc.element.core-js._typed_buffer.ArrayBuffer)
1.  [function <span class="apidocSignatureSpan">core-js._typed_buffer.</span>DataView ()](#apidoc.element.core-js._typed_buffer.DataView)

#### [module core-js._wks_ext](#apidoc.module.core-js._wks_ext)
1.  [function <span class="apidocSignatureSpan">core-js._wks_ext.</span>f (name)](#apidoc.element.core-js._wks_ext.f)

#### [module core-js.core](#apidoc.module.core-js.core)
1.  [function <span class="apidocSignatureSpan">core-js.core.</span>getIterator (it)](#apidoc.element.core-js.core.getIterator)
1.  [function <span class="apidocSignatureSpan">core-js.core.</span>getIteratorMethod (it)](#apidoc.element.core-js.core.getIteratorMethod)
1.  [function <span class="apidocSignatureSpan">core-js.core.</span>inspectSource (it)](#apidoc.element.core-js.core.inspectSource)
1.  [function <span class="apidocSignatureSpan">core-js.core.</span>isIterable (it)](#apidoc.element.core-js.core.isIterable)
1.  object <span class="apidocSignatureSpan">core-js.core.</span>Array
1.  object <span class="apidocSignatureSpan">core-js.core.</span>Date
1.  object <span class="apidocSignatureSpan">core-js.core.</span>Error
1.  object <span class="apidocSignatureSpan">core-js.core.</span>Function
1.  object <span class="apidocSignatureSpan">core-js.core.</span>JSON
1.  object <span class="apidocSignatureSpan">core-js.core.</span>Math
1.  object <span class="apidocSignatureSpan">core-js.core.</span>Number
1.  object <span class="apidocSignatureSpan">core-js.core.</span>Object
1.  object <span class="apidocSignatureSpan">core-js.core.</span>Reflect
1.  object <span class="apidocSignatureSpan">core-js.core.</span>RegExp
1.  object <span class="apidocSignatureSpan">core-js.core.</span>String
1.  object <span class="apidocSignatureSpan">core-js.core.</span>System
1.  object <span class="apidocSignatureSpan">core-js.core.</span>_
1.  object <span class="apidocSignatureSpan">core-js.core.</span>prototype
1.  string <span class="apidocSignatureSpan">core-js.core.</span>version

#### [module core-js.es6_array_iterator](#apidoc.module.core-js.es6_array_iterator)
1.  [function <span class="apidocSignatureSpan">core-js.es6_array_iterator.</span>entries ()](#apidoc.element.core-js.es6_array_iterator.entries)
1.  [function <span class="apidocSignatureSpan">core-js.es6_array_iterator.</span>keys ()](#apidoc.element.core-js.es6_array_iterator.keys)
1.  [function <span class="apidocSignatureSpan">core-js.es6_array_iterator.</span>values ()](#apidoc.element.core-js.es6_array_iterator.values)

#### [module core-js.library](#apidoc.module.core-js.library)
1.  [function <span class="apidocSignatureSpan">core-js.library.</span>ArrayBuffer (a, b, c)](#apidoc.element.core-js.library.ArrayBuffer)
1.  [function <span class="apidocSignatureSpan">core-js.library.</span>DataView (a, b, c)](#apidoc.element.core-js.library.DataView)
1.  [function <span class="apidocSignatureSpan">core-js.library.</span>Dict (iterable)](#apidoc.element.core-js.library.Dict)
1.  [function <span class="apidocSignatureSpan">core-js.library.</span>Float32Array (a, b, c)](#apidoc.element.core-js.library.Float32Array)
1.  [function <span class="apidocSignatureSpan">core-js.library.</span>Float64Array (a, b, c)](#apidoc.element.core-js.library.Float64Array)
1.  [function <span class="apidocSignatureSpan">core-js.library.</span>Int16Array (a, b, c)](#apidoc.element.core-js.library.Int16Array)
1.  [function <span class="apidocSignatureSpan">core-js.library.</span>Int32Array (a, b, c)](#apidoc.element.core-js.library.Int32Array)
1.  [function <span class="apidocSignatureSpan">core-js.library.</span>Int8Array (a, b, c)](#apidoc.element.core-js.library.Int8Array)
1.  [function <span class="apidocSignatureSpan">core-js.library.</span>Map ()](#apidoc.element.core-js.library.Map)
1.  [function <span class="apidocSignatureSpan">core-js.library.</span>Observable ()](#apidoc.element.core-js.library.Observable)
1.  [function <span class="apidocSignatureSpan">core-js.library.</span>Promise (a, b, c)](#apidoc.element.core-js.library.Promise)
1.  [function <span class="apidocSignatureSpan">core-js.library.</span>Set ()](#apidoc.element.core-js.library.Set)
1.  [function <span class="apidocSignatureSpan">core-js.library.</span>Symbol (a, b, c)](#apidoc.element.core-js.library.Symbol)
1.  [function <span class="apidocSignatureSpan">core-js.library.</span>Uint16Array (a, b, c)](#apidoc.element.core-js.library.Uint16Array)
1.  [function <span class="apidocSignatureSpan">core-js.library.</span>Uint32Array (a, b, c)](#apidoc.element.core-js.library.Uint32Array)
1.  [function <span class="apidocSignatureSpan">core-js.library.</span>Uint8Array (a, b, c)](#apidoc.element.core-js.library.Uint8Array)
1.  [function <span class="apidocSignatureSpan">core-js.library.</span>Uint8ClampedArray (a, b, c)](#apidoc.element.core-js.library.Uint8ClampedArray)
1.  [function <span class="apidocSignatureSpan">core-js.library.</span>WeakMap ()](#apidoc.element.core-js.library.WeakMap)
1.  [function <span class="apidocSignatureSpan">core-js.library.</span>WeakSet ()](#apidoc.element.core-js.library.WeakSet)
1.  [function <span class="apidocSignatureSpan">core-js.library.</span>asap ()](#apidoc.element.core-js.library.asap)
1.  [function <span class="apidocSignatureSpan">core-js.library.</span>clearImmediate ()](#apidoc.element.core-js.library.clearImmediate)
1.  [function <span class="apidocSignatureSpan">core-js.library.</span>delay (time)](#apidoc.element.core-js.library.delay)
1.  [function <span class="apidocSignatureSpan">core-js.library.</span>getIterator (it)](#apidoc.element.core-js.library.getIterator)
1.  [function <span class="apidocSignatureSpan">core-js.library.</span>getIteratorMethod (it)](#apidoc.element.core-js.library.getIteratorMethod)
1.  [function <span class="apidocSignatureSpan">core-js.library.</span>isIterable (it)](#apidoc.element.core-js.library.isIterable)
1.  [function <span class="apidocSignatureSpan">core-js.library.</span>parseFloat ()](#apidoc.element.core-js.library.parseFloat)
1.  [function <span class="apidocSignatureSpan">core-js.library.</span>parseInt ()](#apidoc.element.core-js.library.parseInt)
1.  [function <span class="apidocSignatureSpan">core-js.library.</span>setImmediate ()](#apidoc.element.core-js.library.setImmediate)
1.  [function <span class="apidocSignatureSpan">core-js.library.</span>setInterval ()](#apidoc.element.core-js.library.setInterval)
1.  [function <span class="apidocSignatureSpan">core-js.library.</span>setTimeout ()](#apidoc.element.core-js.library.setTimeout)
1.  object <span class="apidocSignatureSpan">core-js.library.</span>Array
1.  object <span class="apidocSignatureSpan">core-js.library.</span>Date
1.  object <span class="apidocSignatureSpan">core-js.library.</span>Error
1.  object <span class="apidocSignatureSpan">core-js.library.</span>Function
1.  object <span class="apidocSignatureSpan">core-js.library.</span>JSON
1.  object <span class="apidocSignatureSpan">core-js.library.</span>Math
1.  object <span class="apidocSignatureSpan">core-js.library.</span>Number
1.  object <span class="apidocSignatureSpan">core-js.library.</span>Object
1.  object <span class="apidocSignatureSpan">core-js.library.</span>Reflect
1.  object <span class="apidocSignatureSpan">core-js.library.</span>RegExp
1.  object <span class="apidocSignatureSpan">core-js.library.</span>String
1.  object <span class="apidocSignatureSpan">core-js.library.</span>System
1.  object <span class="apidocSignatureSpan">core-js.library.</span>_
1.  string <span class="apidocSignatureSpan">core-js.library.</span>version

#### [module core-js.shim](#apidoc.module.core-js.shim)
1.  [function <span class="apidocSignatureSpan">core-js.shim.</span>getIteratorMethod (it)](#apidoc.element.core-js.shim.getIteratorMethod)
1.  [function <span class="apidocSignatureSpan">core-js.shim.</span>inspectSource (it)](#apidoc.element.core-js.shim.inspectSource)
1.  object <span class="apidocSignatureSpan">core-js.shim.</span>Array
1.  object <span class="apidocSignatureSpan">core-js.shim.</span>Date
1.  object <span class="apidocSignatureSpan">core-js.shim.</span>Error
1.  object <span class="apidocSignatureSpan">core-js.shim.</span>Function
1.  object <span class="apidocSignatureSpan">core-js.shim.</span>JSON
1.  object <span class="apidocSignatureSpan">core-js.shim.</span>Math
1.  object <span class="apidocSignatureSpan">core-js.shim.</span>Number
1.  object <span class="apidocSignatureSpan">core-js.shim.</span>Object
1.  object <span class="apidocSignatureSpan">core-js.shim.</span>Reflect
1.  object <span class="apidocSignatureSpan">core-js.shim.</span>String
1.  object <span class="apidocSignatureSpan">core-js.shim.</span>System
1.  object <span class="apidocSignatureSpan">core-js.shim.</span>prototype
1.  string <span class="apidocSignatureSpan">core-js.shim.</span>version



# <a name="apidoc.module.core-js"></a>[module core-js](#apidoc.module.core-js)

#### <a name="apidoc.element.core-js._string_trim"></a>[function <span class="apidocSignatureSpan">core-js.</span>_string_trim (KEY, exec, ALIAS)](#apidoc.element.core-js._string_trim)
- description and source-code
```javascript
_string_trim = function (KEY, exec, ALIAS){
  var exp   = {};
  var FORCE = fails(function(){
    return !!spaces[KEY]() || non[KEY]() != non;
  });
  var fn = exp[KEY] = FORCE ? exec(trim) : spaces[KEY];
  if(ALIAS)exp[ALIAS] = fn;
  $export($export.P + $export.F * FORCE, 'String', exp);
}
```
- example usage
```shell
n/a
```

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
...
	  }
	});

/***/ },
/* 176 */
/***/ function(module, exports, __webpack_require__) {

	// 22.1.3.3 Array.prototype.copyWithin(target, start, end = this.length)
	var $export = __webpack_require__(6);

	$export($export.P, 'Array', {copyWithin: __webpack_require__(177)});

	__webpack_require__(178)('copyWithin');

/***/ },
...
```

#### <a name="apidoc.element.core-js.Array.prototype.entries"></a>[function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>entries ()](#apidoc.element.core-js.Array.prototype.entries)
- description and source-code
```javascript
function entries() { [native code] }
```
- example usage
```shell
...

	'use strict';
	var addToUnscopables = __webpack_require__(178)
	  , step             = __webpack_require__(184)
	  , Iterators        = __webpack_require__(135)
	  , toIObject        = __webpack_require__(30);

	// 22.1.3.4 Array.prototype.entries()
	// 22.1.3.13 Array.prototype.keys()
	// 22.1.3.29 Array.prototype.values()
	// 22.1.3.30 Array.prototype[@@iterator]()
	module.exports = __webpack_require__(134)(Array, 'Array', function(iterated, kind){
	  this._t = toIObject(iterated); // target
	  this._i = 0;                   // next index
	  this._k = kind;                // kind
...
```

#### <a name="apidoc.element.core-js.Array.prototype.every"></a>[function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>every ()](#apidoc.element.core-js.Array.prototype.every)
- description and source-code
```javascript
function every() { [native code] }
```
- example usage
```shell
...
/***/ function(module, exports, __webpack_require__) {

	'use strict';
	var $export = __webpack_require__(6)
	  , $every  = __webpack_require__(164)(4);

	$export($export.P + $export.F * !__webpack_require__(160)([].every, true), 'Array', {
	  // 22.1.3.5 / 15.4.4.16 Array.prototype.every(callbackfn [, thisArg])
	  every: function every(callbackfn /* , thisArg */){
	    return $every(this, callbackfn, arguments[1]);
	  }
	});

/***/ },
/* 171 */
...
```

#### <a name="apidoc.element.core-js.Array.prototype.fill"></a>[function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>fill ()](#apidoc.element.core-js.Array.prototype.fill)
- description and source-code
```javascript
function fill() { [native code] }
```
- example usage
```shell
...
	  ArrayProto[UNSCOPABLES][key] = true;
	};

/***/ },
/* 179 */
/***/ function(module, exports, __webpack_require__) {

	// 22.1.3.6 Array.prototype.fill(value, start = 0, end = this.length)
	var $export = __webpack_require__(6);

	$export($export.P, 'Array', {fill: __webpack_require__(180)});

	__webpack_require__(178)('fill');

/***/ },
...
```

#### <a name="apidoc.element.core-js.Array.prototype.filter"></a>[function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>filter ()](#apidoc.element.core-js.Array.prototype.filter)
- description and source-code
```javascript
function filter() { [native code] }
```
- example usage
```shell
...
/***/ function(module, exports, __webpack_require__) {

	'use strict';
	var $export = __webpack_require__(6)
	  , $filter = __webpack_require__(164)(2);

	$export($export.P + $export.F * !__webpack_require__(160)([].filter, true), 'Array', {
	  // 22.1.3.7 / 15.4.4.20 Array.prototype.filter(callbackfn [, thisArg])
	  filter: function filter(callbackfn /* , thisArg */){
	    return $filter(this, callbackfn, arguments[1]);
	  }
	});

/***/ },
/* 169 */
...
```

#### <a name="apidoc.element.core-js.Array.prototype.find"></a>[function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>find ()](#apidoc.element.core-js.Array.prototype.find)
- description and source-code
```javascript
function find() { [native code] }
```
- example usage
```shell
...
	};

/***/ },
/* 181 */
/***/ function(module, exports, __webpack_require__) {

	'use strict';
	// 22.1.3.8 Array.prototype.find(predicate, thisArg = undefined)
	var $export = __webpack_require__(6)
	  , $find   = __webpack_require__(164)(5)
	  , KEY     = 'find'
	  , forced  = true;
	// Shouldn't skip holes
	if(KEY in [])Array(1)[KEY](function(){ forced = false; });
	$export($export.P + $export.F * forced, 'Array', {
...
```

#### <a name="apidoc.element.core-js.Array.prototype.findIndex"></a>[function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>findIndex ()](#apidoc.element.core-js.Array.prototype.findIndex)
- description and source-code
```javascript
function findIndex() { [native code] }
```
- example usage
```shell
...
	__webpack_require__(178)(KEY);

/***/ },
/* 182 */
/***/ function(module, exports, __webpack_require__) {

	'use strict';
	// 22.1.3.9 Array.prototype.findIndex(predicate, thisArg = undefined)
	var $export = __webpack_require__(6)
	  , $find   = __webpack_require__(164)(6)
	  , KEY     = 'findIndex'
	  , forced  = true;
	// Shouldn't skip holes
	if(KEY in [])Array(1)[KEY](function(){ forced = false; });
	$export($export.P + $export.F * forced, 'Array', {
...
```

#### <a name="apidoc.element.core-js.Array.prototype.forEach"></a>[function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>forEach ()](#apidoc.element.core-js.Array.prototype.forEach)
- description and source-code
```javascript
function forEach() { [native code] }
```
- example usage
```shell
...
	// should work with symbols and should have deterministic property order (V8 bug)
	module.exports = !$assign || __webpack_require__(5)(function(){
	  var A = {}
	    , B = {}
	    , S = Symbol()
	    , K = 'abcdefghijklmnopqrst';
	  A[S] = 7;
	  K.split('').forEach(function(k){ B[k] = k; });
	  return $assign({}, A)[S] != 7 || Object.keys($assign({}, B)).join('') != K;
	}) ? function assign(target, source){ // eslint-disable-line no-unused-vars
	  var T     = toObject(target)
	    , aLen  = arguments.length
	    , index = 1
	    , getSymbols = gOPS.f
	    , isEnum     = pIE.f;
...
```

#### <a name="apidoc.element.core-js.Array.prototype.includes"></a>[function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>includes ()](#apidoc.element.core-js.Array.prototype.includes)
- description and source-code
```javascript
function includes() { [native code] }
```
- example usage
```shell
...
	  } return true;
	};

/***/ },
/* 130 */
/***/ function(module, exports, __webpack_require__) {

	// 21.1.3.7 String.prototype.includes(searchString, position = 0)
	'use strict';
	var $export  = __webpack_require__(6)
	  , context  = __webpack_require__(127)
	  , INCLUDES = 'includes';

	$export($export.P + $export.F * __webpack_require__(129)(INCLUDES), 'String', {
	  includes: function includes(searchString /*, position = 0 */){
...
```

#### <a name="apidoc.element.core-js.Array.prototype.indexOf"></a>[function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>indexOf ()](#apidoc.element.core-js.Array.prototype.indexOf)
- description and source-code
```javascript
function indexOf() { [native code] }
```
- example usage
```shell
...
	var $export  = __webpack_require__(6)
	  , context  = __webpack_require__(127)
	  , INCLUDES = 'includes';

	$export($export.P + $export.F * __webpack_require__(129)(INCLUDES), 'String', {
	  includes: function includes(searchString /*, position = 0 */){
	    return !!~context(this, searchString, INCLUDES)
	      .indexOf(searchString, arguments.length > 1 ? arguments[1] : undefined);
	  }
	});

/***/ },
/* 131 */
/***/ function(module, exports, __webpack_require__) {
...
```

#### <a name="apidoc.element.core-js.Array.prototype.join"></a>[function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>join ()](#apidoc.element.core-js.Array.prototype.join)
- description and source-code
```javascript
function join() { [native code] }
```
- example usage
```shell
...
	  return $toString.call(it);
	};

	(module.exports = function(O, key, val, safe){
	  var isFunction = typeof val == 'function';
	  if(isFunction)has(val, 'name') || hide(val, 'name', key);
	  if(O[key] === val)return;
	  if(isFunction)has(val, SRC) || hide(val, SRC, O[key] ? '' + O[key] : TPL.join(String(key)));
	  if(O === global){
	    O[key] = val;
	  } else {
	    if(!safe){
	      delete O[key];
	      hide(O, key, val);
	    } else {
...
```

#### <a name="apidoc.element.core-js.Array.prototype.keys"></a>[function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>keys ()](#apidoc.element.core-js.Array.prototype.keys)
- description and source-code
```javascript
function keys() { [native code] }
```
- example usage
```shell
...
	  while(length > index)if(O[key = keys[index++]] === el)return key;
	};

/***/ },
/* 28 */
/***/ function(module, exports, __webpack_require__) {

	// 19.1.2.14 / 15.2.3.14 Object.keys(O)
	var $keys       = __webpack_require__(29)
	  , enumBugKeys = __webpack_require__(39);

	module.exports = Object.keys || function keys(O){
	  return $keys(O, enumBugKeys);
	};
...
```

#### <a name="apidoc.element.core-js.Array.prototype.lastIndexOf"></a>[function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>lastIndexOf ()](#apidoc.element.core-js.Array.prototype.lastIndexOf)
- description and source-code
```javascript
function lastIndexOf() { [native code] }
```
- example usage
```shell
...

	'use strict';
	var $export       = __webpack_require__(6)
	  , toIObject     = __webpack_require__(30)
	  , toInteger     = __webpack_require__(36)
	  , toLength      = __webpack_require__(35)
	  , $native       = [].lastIndexOf
	  , NEGATIVE_ZERO = !!$native && 1 / [1].lastIndexOf(1, -0) < 0;

	$export($export.P + $export.F * (NEGATIVE_ZERO || !__webpack_require__(160)($native)), 'Array', {
	  // 22.1.3.14 / 15.4.4.15 Array.prototype.lastIndexOf(searchElement [, fromIndex])
	  lastIndexOf: function lastIndexOf(searchElement /*, fromIndex = @[*-1] */){
	    // convert -0 to +0
	    if(NEGATIVE_ZERO)return $native.apply(this, arguments) || 0;
	    var O      = toIObject(this)
...
```

#### <a name="apidoc.element.core-js.Array.prototype.map"></a>[function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>map ()](#apidoc.element.core-js.Array.prototype.map)
- description and source-code
```javascript
function map() { [native code] }
```
- example usage
```shell
...
/***/ function(module, exports, __webpack_require__) {

	'use strict';
	var $export = __webpack_require__(6)
	  , $map    = __webpack_require__(164)(1);

	$export($export.P + $export.F * !__webpack_require__(160)([].map, true), 'Array', {
	  // 22.1.3.15 / 15.4.4.19 Array.prototype.map(callbackfn [, thisArg])
	  map: function map(callbackfn /* , thisArg */){
	    return $map(this, callbackfn, arguments[1]);
	  }
	});

/***/ },
/* 168 */
...
```

#### <a name="apidoc.element.core-js.Array.prototype.reduce"></a>[function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>reduce ()](#apidoc.element.core-js.Array.prototype.reduce)
- description and source-code
```javascript
function reduce() { [native code] }
```
- example usage
```shell
...
/***/ function(module, exports, __webpack_require__) {

	'use strict';
	var $export = __webpack_require__(6)
	  , $reduce = __webpack_require__(172);

	$export($export.P + $export.F * !__webpack_require__(160)([].reduce, true), 'Array', {
	  // 22.1.3.18 / 15.4.4.21 Array.prototype.reduce(callbackfn [, initialValue])
	  reduce: function reduce(callbackfn /* , initialValue */){
	    return $reduce(this, callbackfn, arguments.length, arguments[1], false);
	  }
	});

/***/ },
/* 172 */
...
```

#### <a name="apidoc.element.core-js.Array.prototype.reduceRight"></a>[function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>reduceRight ()](#apidoc.element.core-js.Array.prototype.reduceRight)
- description and source-code
```javascript
function reduceRight() { [native code] }
```
- example usage
```shell
...
/***/ function(module, exports, __webpack_require__) {

	'use strict';
	var $export = __webpack_require__(6)
	  , $reduce = __webpack_require__(172);

	$export($export.P + $export.F * !__webpack_require__(160)([].reduceRight, true), 'Array', {
	  // 22.1.3.19 / 15.4.4.22 Array.prototype.reduceRight(callbackfn [, initialValue])
	  reduceRight: function reduceRight(callbackfn /* , initialValue */){
	    return $reduce(this, callbackfn, arguments.length, arguments[1], true);
	  }
	});

/***/ },
/* 174 */
...
```

#### <a name="apidoc.element.core-js.Array.prototype.slice"></a>[function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>slice ()](#apidoc.element.core-js.Array.prototype.slice)
- description and source-code
```javascript
function slice() { [native code] }
```
- example usage
```shell
...
/***/ },
/* 32 */
/***/ function(module, exports) {

	var toString = {}.toString;

	module.exports = function(it){
	  return toString.call(it).slice(8, -1);
	};

/***/ },
/* 33 */
/***/ function(module, exports) {

	// 7.2.1 RequireObjectCoercible(argument)
...
```

#### <a name="apidoc.element.core-js.Array.prototype.some"></a>[function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>some ()](#apidoc.element.core-js.Array.prototype.some)
- description and source-code
```javascript
function some() { [native code] }
```
- example usage
```shell
...
/***/ function(module, exports, __webpack_require__) {

	'use strict';
	var $export = __webpack_require__(6)
	  , $some   = __webpack_require__(164)(3);

	$export($export.P + $export.F * !__webpack_require__(160)([].some, true), 'Array', {
	  // 22.1.3.23 / 15.4.4.17 Array.prototype.some(callbackfn [, thisArg])
	  some: function some(callbackfn /* , thisArg */){
	    return $some(this, callbackfn, arguments[1]);
	  }
	});

/***/ },
/* 170 */
...
```

#### <a name="apidoc.element.core-js.Array.prototype.sort"></a>[function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>sort ()](#apidoc.element.core-js.Array.prototype.sort)
- description and source-code
```javascript
function sort() { [native code] }
```
- example usage
```shell
...
	  , toObject  = __webpack_require__(56)
	  , fails     = __webpack_require__(5)
	  , $sort     = [].sort
	  , test      = [1, 2, 3];

	$export($export.P + $export.F * (fails(function(){
	  // IE8-
	  test.sort(undefined);
	}) || !fails(function(){
	  // V8 bug
	  test.sort(null);
	  // Old WebKit
	}) || !__webpack_require__(160)($sort)), 'Array', {
	  // 22.1.3.25 Array.prototype.sort(comparefn)
	  sort: function sort(comparefn){
...
```

#### <a name="apidoc.element.core-js.Array.prototype.values"></a>[function <span class="apidocSignatureSpan">core-js.Array.prototype.</span>values ()](#apidoc.element.core-js.Array.prototype.values)
- description and source-code
```javascript
function values() { [native code] }
```
- example usage
```shell
...
	var addToUnscopables = __webpack_require__(178)
	  , step             = __webpack_require__(184)
	  , Iterators        = __webpack_require__(135)
	  , toIObject        = __webpack_require__(30);

	// 22.1.3.4 Array.prototype.entries()
	// 22.1.3.13 Array.prototype.keys()
	// 22.1.3.29 Array.prototype.values()
	// 22.1.3.30 Array.prototype[@@iterator]()
	module.exports = __webpack_require__(134)(Array, 'Array', function(iterated, kind){
	  this._t = toIObject(iterated); // target
	  this._i = 0;                   // next index
	  this._k = kind;                // kind
	// 22.1.5.2.1 %ArrayIteratorPrototype%.next()
	}, function(){
...
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
...

	$export($export.P + $export.F * __webpack_require__(5)(function(){
	  return new Date(NaN).toJSON() !== null || Date.prototype.toJSON.call({toISOString: function(){ return 1; }}) !== 1;
	}), 'Date', {
	  toJSON: function toJSON(key){
	    var O  = toObject(this)
	      , pv = toPrimitive(O);
	    return typeof pv == 'number' && !isFinite(pv) ? null : O.toISOString();
	  }
	});

/***/ },
/* 227 */
/***/ function(module, exports, __webpack_require__) {
...
```

#### <a name="apidoc.element.core-js.Date.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">core-js.Date.prototype.</span>toJSON ()](#apidoc.element.core-js.Date.prototype.toJSON)
- description and source-code
```javascript
function toJSON() { [native code] }
```
- example usage
```shell
...

	'use strict';
	var $export     = __webpack_require__(6)
	  , toObject    = __webpack_require__(56)
	  , toPrimitive = __webpack_require__(14);

	$export($export.P + $export.F * __webpack_require__(5)(function(){
	  return new Date(NaN).toJSON() !== null || Date.prototype.toJSON.call({toISOString: function(){ return 1; }}) !== 1;
	}), 'Date', {
	  toJSON: function toJSON(key){
	    var O  = toObject(this)
	      , pv = toPrimitive(O);
	    return typeof pv == 'number' && !isFinite(pv) ? null : O.toISOString();
	  }
	});
...
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
...
	    : (B = cof(O)) == 'Object' && typeof O.callee == 'function' ? 'Arguments' : B;
	};

/***/ },
/* 74 */
/***/ function(module, exports, __webpack_require__) {

	// 19.2.3.2 / 15.3.4.5 Function.prototype.bind(thisArg, args...)
	var $export = __webpack_require__(6);

	$export($export.P, 'Function', {bind: __webpack_require__(75)});

/***/ },
/* 75 */
/***/ function(module, exports, __webpack_require__) {
...
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
...
	  while(x2 >= 2){
	    n  += 1;
	    x2 /= 2;
	  } return n;
	};

	$export($export.P + $export.F * (!!$toFixed && (
	  0.00008.toFixed(3) !== '0.000' ||
	  0.9.toFixed(0) !== '1' ||
	  1.255.toFixed(2) !== '1.25' ||
	  1000000000000000128..toFixed(0) !== '1000000000000000128'
	) || !__webpack_require__(5)(function(){
	  // V8 ~ Android 4.3-
	  $toFixed.call({});
	})), 'Number', {
...
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
...
	};

/***/ },
/* 137 */
/***/ function(module, exports, __webpack_require__) {

	'use strict';
	// B.2.3.2 String.prototype.anchor(name)
	__webpack_require__(138)('anchor', function(createHTML){
	  return function anchor(name){
	    return createHTML(this, 'a', 'name', name);
	  }
	});

/***/ },
...
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
...
	};

/***/ },
/* 139 */
/***/ function(module, exports, __webpack_require__) {

	'use strict';
	// B.2.3.3 String.prototype.big()
	__webpack_require__(138)('big', function(createHTML){
	  return function big(){
	    return createHTML(this, 'big', '', '');
	  }
	});

/***/ },
...
```

#### <a name="apidoc.element.core-js.String.prototype.blink"></a>[function <span class="apidocSignatureSpan">core-js.String.prototype.</span>blink ()](#apidoc.element.core-js.String.prototype.blink)
- description and source-code
```javascript
function blink() { [native code] }
```
- example usage
```shell
...
	});

/***/ },
/* 140 */
/***/ function(module, exports, __webpack_require__) {

	'use strict';
	// B.2.3.4 String.prototype.blink()
	__webpack_require__(138)('blink', function(createHTML){
	  return function blink(){
	    return createHTML(this, 'blink', '', '');
	  }
	});

/***/ },
...
```

#### <a name="apidoc.element.core-js.String.prototype.bold"></a>[function <span class="apidocSignatureSpan">core-js.String.prototype.</span>bold ()](#apidoc.element.core-js.String.prototype.bold)
- description and source-code
```javascript
function bold() { [native code] }
```
- example usage
```shell
...
	});

/***/ },
/* 141 */
/***/ function(module, exports, __webpack_require__) {

	'use strict';
	// B.2.3.5 String.prototype.bold()
	__webpack_require__(138)('bold', function(createHTML){
	  return function bold(){
	    return createHTML(this, 'b', '', '');
	  }
	});

/***/ },
...
```

#### <a name="apidoc.element.core-js.String.prototype.codePointAt"></a>[function <span class="apidocSignatureSpan">core-js.String.prototype.</span>codePointAt ()](#apidoc.element.core-js.String.prototype.codePointAt)
- description and source-code
```javascript
function codePointAt() { [native code] }
```
- example usage
```shell
...
/* 124 */
/***/ function(module, exports, __webpack_require__) {

	'use strict';
	var $export = __webpack_require__(6)
	  , $at     = __webpack_require__(125)(false);
	$export($export.P, 'String', {
	  // 21.1.3.3 String.prototype.codePointAt(pos)
	  codePointAt: function codePointAt(pos){
	    return $at(this, pos);
	  }
	});

/***/ },
/* 125 */
...
```

#### <a name="apidoc.element.core-js.String.prototype.endsWith"></a>[function <span class="apidocSignatureSpan">core-js.String.prototype.</span>endsWith ()](#apidoc.element.core-js.String.prototype.endsWith)
- description and source-code
```javascript
function endsWith() { [native code] }
```
- example usage
```shell
...
	  };
	};

/***/ },
/* 126 */
/***/ function(module, exports, __webpack_require__) {

	// 21.1.3.6 String.prototype.endsWith(searchString [, endPosition])
	'use strict';
	var $export   = __webpack_require__(6)
	  , toLength  = __webpack_require__(35)
	  , context   = __webpack_require__(127)
	  , ENDS_WITH = 'endsWith'
	  , $endsWith = ''[ENDS_WITH];
...
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
...
	});

/***/ },
/* 142 */
/***/ function(module, exports, __webpack_require__) {

	'use strict';
	// B.2.3.6 String.prototype.fixed()
	__webpack_require__(138)('fixed', function(createHTML){
	  return function fixed(){
	    return createHTML(this, 'tt', '', '');
	  }
	});

/***/ },
...
```

#### <a name="apidoc.element.core-js.String.prototype.fontcolor"></a>[function <span class="apidocSignatureSpan">core-js.String.prototype.</span>fontcolor ()](#apidoc.element.core-js.String.prototype.fontcolor)
- description and source-code
```javascript
function fontcolor() { [native code] }
```
- example usage
```shell
...
	});

/***/ },
/* 143 */
/***/ function(module, exports, __webpack_require__) {

	'use strict';
	// B.2.3.7 String.prototype.fontcolor(color)
	__webpack_require__(138)('fontcolor', function(createHTML){
	  return function fontcolor(color){
	    return createHTML(this, 'font', 'color', color);
	  }
	});

/***/ },
...
```

#### <a name="apidoc.element.core-js.String.prototype.fontsize"></a>[function <span class="apidocSignatureSpan">core-js.String.prototype.</span>fontsize ()](#apidoc.element.core-js.String.prototype.fontsize)
- description and source-code
```javascript
function fontsize() { [native code] }
```
- example usage
```shell
...
	});

/***/ },
/* 144 */
/***/ function(module, exports, __webpack_require__) {

	'use strict';
	// B.2.3.8 String.prototype.fontsize(size)
	__webpack_require__(138)('fontsize', function(createHTML){
	  return function fontsize(size){
	    return createHTML(this, 'font', 'size', size);
	  }
	});

/***/ },
...
```

#### <a name="apidoc.element.core-js.String.prototype.includes"></a>[function <span class="apidocSignatureSpan">core-js.String.prototype.</span>includes ()](#apidoc.element.core-js.String.prototype.includes)
- description and source-code
```javascript
function includes() { [native code] }
```
- example usage
```shell
...
	  } return true;
	};

/***/ },
/* 130 */
/***/ function(module, exports, __webpack_require__) {

	// 21.1.3.7 String.prototype.includes(searchString, position = 0)
	'use strict';
	var $export  = __webpack_require__(6)
	  , context  = __webpack_require__(127)
	  , INCLUDES = 'includes';

	$export($export.P + $export.F * __webpack_require__(129)(INCLUDES), 'String', {
	  includes: function includes(searchString /*, position = 0 */){
...
```

#### <a name="apidoc.element.core-js.String.prototype.italics"></a>[function <span class="apidocSignatureSpan">core-js.String.prototype.</span>italics ()](#apidoc.element.core-js.String.prototype.italics)
- description and source-code
```javascript
function italics() { [native code] }
```
- example usage
```shell
...
	});

/***/ },
/* 145 */
/***/ function(module, exports, __webpack_require__) {

	'use strict';
	// B.2.3.9 String.prototype.italics()
	__webpack_require__(138)('italics', function(createHTML){
	  return function italics(){
	    return createHTML(this, 'i', '', '');
	  }
	});

/***/ },
...
```

#### <a name="apidoc.element.core-js.String.prototype.link"></a>[function <span class="apidocSignatureSpan">core-js.String.prototype.</span>link ()](#apidoc.element.core-js.String.prototype.link)
- description and source-code
```javascript
function link() { [native code] }
```
- example usage
```shell
...
	});

/***/ },
/* 146 */
/***/ function(module, exports, __webpack_require__) {

	'use strict';
	// B.2.3.10 String.prototype.link(url)
	__webpack_require__(138)('link', function(createHTML){
	  return function link(url){
	    return createHTML(this, 'a', 'href', url);
	  }
	});

/***/ },
...
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
...
/***/ },
/* 131 */
/***/ function(module, exports, __webpack_require__) {

	var $export = __webpack_require__(6);

	$export($export.P, 'String', {
	  // 21.1.3.13 String.prototype.repeat(count)
	  repeat: __webpack_require__(85)
	});

/***/ },
/* 132 */
/***/ function(module, exports, __webpack_require__) {
...
```

#### <a name="apidoc.element.core-js.String.prototype.small"></a>[function <span class="apidocSignatureSpan">core-js.String.prototype.</span>small ()](#apidoc.element.core-js.String.prototype.small)
- description and source-code
```javascript
function small() { [native code] }
```
- example usage
```shell
...
	});

/***/ },
/* 147 */
/***/ function(module, exports, __webpack_require__) {

	'use strict';
	// B.2.3.11 String.prototype.small()
	__webpack_require__(138)('small', function(createHTML){
	  return function small(){
	    return createHTML(this, 'small', '', '');
	  }
	});

/***/ },
...
```

#### <a name="apidoc.element.core-js.String.prototype.startsWith"></a>[function <span class="apidocSignatureSpan">core-js.String.prototype.</span>startsWith ()](#apidoc.element.core-js.String.prototype.startsWith)
- description and source-code
```javascript
function startsWith() { [native code] }
```
- example usage
```shell
...
	  repeat: __webpack_require__(85)
	});

/***/ },
/* 132 */
/***/ function(module, exports, __webpack_require__) {

	// 21.1.3.18 String.prototype.startsWith(searchString [, position ])
	'use strict';
	var $export     = __webpack_require__(6)
	  , toLength    = __webpack_require__(35)
	  , context     = __webpack_require__(127)
	  , STARTS_WITH = 'startsWith'
	  , $startsWith = ''[STARTS_WITH];
...
```

#### <a name="apidoc.element.core-js.String.prototype.strike"></a>[function <span class="apidocSignatureSpan">core-js.String.prototype.</span>strike ()](#apidoc.element.core-js.String.prototype.strike)
- description and source-code
```javascript
function strike() { [native code] }
```
- example usage
```shell
...
	});

/***/ },
/* 148 */
/***/ function(module, exports, __webpack_require__) {

	'use strict';
	// B.2.3.12 String.prototype.strike()
	__webpack_require__(138)('strike', function(createHTML){
	  return function strike(){
	    return createHTML(this, 'strike', '', '');
	  }
	});

/***/ },
...
```

#### <a name="apidoc.element.core-js.String.prototype.sub"></a>[function <span class="apidocSignatureSpan">core-js.String.prototype.</span>sub ()](#apidoc.element.core-js.String.prototype.sub)
- description and source-code
```javascript
function sub() { [native code] }
```
- example usage
```shell
...
	});

/***/ },
/* 149 */
/***/ function(module, exports, __webpack_require__) {

	'use strict';
	// B.2.3.13 String.prototype.sub()
	__webpack_require__(138)('sub', function(createHTML){
	  return function sub(){
	    return createHTML(this, 'sub', '', '');
	  }
	});

/***/ },
...
```

#### <a name="apidoc.element.core-js.String.prototype.sup"></a>[function <span class="apidocSignatureSpan">core-js.String.prototype.</span>sup ()](#apidoc.element.core-js.String.prototype.sup)
- description and source-code
```javascript
function sup() { [native code] }
```
- example usage
```shell
...
	});

/***/ },
/* 150 */
/***/ function(module, exports, __webpack_require__) {

	'use strict';
	// B.2.3.14 String.prototype.sup()
	__webpack_require__(138)('sup', function(createHTML){
	  return function sup(){
	    return createHTML(this, 'sup', '', '');
	  }
	});

/***/ },
...
```

#### <a name="apidoc.element.core-js.String.prototype.trim"></a>[function <span class="apidocSignatureSpan">core-js.String.prototype.</span>trim ()](#apidoc.element.core-js.String.prototype.trim)
- description and source-code
```javascript
function trim() { [native code] }
```
- example usage
```shell
...
	  , BROKEN_COF        = cof(__webpack_require__(44)(proto)) == NUMBER
	  , TRIM              = 'trim' in String.prototype;

	// 7.1.3 ToNumber(argument)
	var toNumber = function(argument){
	  var it = toPrimitive(argument, false);
	  if(typeof it == 'string' && it.length > 2){
	    it = TRIM ? it.trim() : $trim(it, 3);
	    var first = it.charCodeAt(0)
	      , third, radix, maxCode;
	    if(first === 43 || first === 45){
	      third = it.charCodeAt(2);
	      if(third === 88 || third === 120)return NaN; // Number('+0x1') should be NaN, old V8 fix
	    } else if(first === 48){
	      switch(it.charCodeAt(1)){
...
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



# <a name="apidoc.module.core-js._collection_strong"></a>[module core-js._collection_strong](#apidoc.module.core-js._collection_strong)

#### <a name="apidoc.element.core-js._collection_strong.def"></a>[function <span class="apidocSignatureSpan">core-js._collection_strong.</span>def (that, key, value)](#apidoc.element.core-js._collection_strong.def)
- description and source-code
```javascript
def = function (that, key, value){
  var entry = getEntry(that, key)
    , prev, index;
  // change existing entry
  if(entry){
    entry.v = value;
  // create new entry
  } else {
    that._l = entry = {
      i: index = fastKey(key, true), // <- index
      k: key,                        // <- key
      v: value,                      // <- value
      p: prev = that._l,             // <- previous entry
      n: undefined,                  // <- next entry
      r: false                       // <- removed
    };
    if(!that._f)that._f = entry;
    if(prev)prev.n = entry;
    that[SIZE]++;
    // add to index
    if(index !== 'F')that._i[index] = entry;
  } return that;
}
```
- example usage
```shell
...
	  // 23.1.3.6 Map.prototype.get(key)
	  get: function get(key){
	    var entry = strong.getEntry(this, key);
	    return entry && entry.v;
	  },
	  // 23.1.3.9 Map.prototype.set(key, value)
	  set: function set(key, value){
	    return strong.def(this, key === 0 ? 0 : key, value);
	  }
	}, strong, true);

/***/ },
/* 204 */
/***/ function(module, exports, __webpack_require__) {
...
```

#### <a name="apidoc.element.core-js._collection_strong.getConstructor"></a>[function <span class="apidocSignatureSpan">core-js._collection_strong.</span>getConstructor (wrapper, NAME, IS_MAP, ADDER)](#apidoc.element.core-js._collection_strong.getConstructor)
- description and source-code
```javascript
getConstructor = function (wrapper, NAME, IS_MAP, ADDER){
  var C = wrapper(function(that, iterable){
    anInstance(that, C, NAME, '_i');
    that._i = create(null); // index
    that._f = undefined;    // first entry
    that._l = undefined;    // last entry
    that[SIZE] = 0;         // size
    if(iterable != undefined)forOf(iterable, IS_MAP, that[ADDER], that);
  });
  redefineAll(C.prototype, {
    // 23.1.3.1 Map.prototype.clear()
    // 23.2.3.2 Set.prototype.clear()
    clear: function clear(){
      for(var that = this, data = that._i, entry = that._f; entry; entry = entry.n){
        entry.r = true;
        if(entry.p)entry.p = entry.p.n = undefined;
        delete data[entry.i];
      }
      that._f = that._l = undefined;
      that[SIZE] = 0;
    },
    // 23.1.3.3 Map.prototype.delete(key)
    // 23.2.3.4 Set.prototype.delete(value)
    'delete': function(key){
      var that  = this
        , entry = getEntry(that, key);
      if(entry){
        var next = entry.n
          , prev = entry.p;
        delete that._i[entry.i];
        entry.r = true;
        if(prev)prev.n = next;
        if(next)next.p = prev;
        if(that._f == entry)that._f = next;
        if(that._l == entry)that._l = prev;
        that[SIZE]--;
      } return !!entry;
    },
    // 23.2.3.6 Set.prototype.forEach(callbackfn, thisArg = undefined)
    // 23.1.3.5 Map.prototype.forEach(callbackfn, thisArg = undefined)
    forEach: function forEach(callbackfn /*, that = undefined */){
      anInstance(this, C, 'forEach');
      var f = ctx(callbackfn, arguments.length > 1 ? arguments[1] : undefined, 3)
        , entry;
      while(entry = entry ? entry.n : this._f){
        f(entry.v, entry.k, this);
        // revert to the last existing entry
        while(entry && entry.r)entry = entry.p;
      }
    },
    // 23.1.3.7 Map.prototype.has(key)
    // 23.2.3.7 Set.prototype.has(value)
    has: function has(key){
      return !!getEntry(this, key);
    }
  });
  if(DESCRIPTORS)dP(C.prototype, 'size', {
    get: function(){
      return defined(this[SIZE]);
    }
  });
  return C;
}
```
- example usage
```shell
...
	        : function set(a, b){ fn.call(this, a === 0 ? 0 : a, b); return this; }
	    );
	  };
	  if(typeof C != 'function' || !(IS_WEAK || proto.forEach && !fails(function(){
	    new C().entries().next();
	  }))){
	    // create collection constructor
	    C = common.getConstructor(wrapper, NAME, IS_MAP, ADDER);
	    redefineAll(C.prototype, methods);
	    meta.NEED = true;
	  } else {
	    var instance             = new C
	      // early implementations not supports chaining
	      , HASNT_CHAINING       = instance[ADDER](IS_WEAK ? {} : -0, 1) != instance
	      // V8 ~  Chromium 40- weak-collections throws on primitives, but should return false
...
```

#### <a name="apidoc.element.core-js._collection_strong.getEntry"></a>[function <span class="apidocSignatureSpan">core-js._collection_strong.</span>getEntry (that, key)](#apidoc.element.core-js._collection_strong.getEntry)
- description and source-code
```javascript
getEntry = function (that, key){
  // fast case
  var index = fastKey(key), entry;
  if(index !== 'F')return that._i[index];
  // frozen object case
  for(entry = that._f; entry; entry = entry.n){
    if(entry.k == key)return entry;
  }
}
```
- example usage
```shell
...

	// 23.1 Map Objects
	module.exports = __webpack_require__(205)('Map', function(get){
	  return function Map(){ return get(this, arguments.length > 0 ? arguments[0] : undefined); };
	}, {
	  // 23.1.3.6 Map.prototype.get(key)
	  get: function get(key){
	    var entry = strong.getEntry(this, key);
	    return entry && entry.v;
	  },
	  // 23.1.3.9 Map.prototype.set(key, value)
	  set: function set(key, value){
	    return strong.def(this, key === 0 ? 0 : key, value);
	  }
	}, strong, true);
...
```

#### <a name="apidoc.element.core-js._collection_strong.setStrong"></a>[function <span class="apidocSignatureSpan">core-js._collection_strong.</span>setStrong (C, NAME, IS_MAP)](#apidoc.element.core-js._collection_strong.setStrong)
- description and source-code
```javascript
setStrong = function (C, NAME, IS_MAP){
  // add .keys, .values, .entries, [@@iterator]
  // 23.1.3.4, 23.1.3.8, 23.1.3.11, 23.1.3.12, 23.2.3.5, 23.2.3.8, 23.2.3.10, 23.2.3.11
  $iterDefine(C, NAME, function(iterated, kind){
    this._t = iterated;  // target
    this._k = kind;      // kind
    this._l = undefined; // previous
  }, function(){
    var that  = this
      , kind  = that._k
      , entry = that._l;
    // revert to the last existing entry
    while(entry && entry.r)entry = entry.p;
    // get next entry
    if(!that._t || !(that._l = entry = entry ? entry.n : that._t._f)){
      // or finish the iteration
      that._t = undefined;
      return step(1);
    }
    // return step by kind
    if(kind == 'keys'  )return step(0, entry.k);
    if(kind == 'values')return step(0, entry.v);
    return step(0, [entry.k, entry.v]);
  }, IS_MAP ? 'entries' : 'values' , !IS_MAP, true);

  // add [@@species], 23.1.2.2, 23.2.2.2
  setSpecies(NAME);
}
```
- example usage
```shell
...
	  }

	  setToStringTag(C, NAME);

	  O[NAME] = C;
	  $export($export.G + $export.W + $export.F * (C != Base), O);

	  if(!IS_WEAK)common.setStrong(C, NAME, IS_MAP);

	  return C;
	};

/***/ },
/* 206 */
/***/ function(module, exports, __webpack_require__) {
...
```



# <a name="apidoc.module.core-js._collection_weak"></a>[module core-js._collection_weak](#apidoc.module.core-js._collection_weak)

#### <a name="apidoc.element.core-js._collection_weak.def"></a>[function <span class="apidocSignatureSpan">core-js._collection_weak.</span>def (that, key, value)](#apidoc.element.core-js._collection_weak.def)
- description and source-code
```javascript
def = function (that, key, value){
  var data = getWeak(anObject(key), true);
  if(data === true)uncaughtFrozenStore(that).set(key, value);
  else data[that._i] = value;
  return that;
}
```
- example usage
```shell
...
	  // 23.1.3.6 Map.prototype.get(key)
	  get: function get(key){
	    var entry = strong.getEntry(this, key);
	    return entry && entry.v;
	  },
	  // 23.1.3.9 Map.prototype.set(key, value)
	  set: function set(key, value){
	    return strong.def(this, key === 0 ? 0 : key, value);
	  }
	}, strong, true);

/***/ },
/* 204 */
/***/ function(module, exports, __webpack_require__) {
...
```

#### <a name="apidoc.element.core-js._collection_weak.getConstructor"></a>[function <span class="apidocSignatureSpan">core-js._collection_weak.</span>getConstructor (wrapper, NAME, IS_MAP, ADDER)](#apidoc.element.core-js._collection_weak.getConstructor)
- description and source-code
```javascript
getConstructor = function (wrapper, NAME, IS_MAP, ADDER){
  var C = wrapper(function(that, iterable){
    anInstance(that, C, NAME, '_i');
    that._i = id++;      // collection id
    that._l = undefined; // leak store for uncaught frozen objects
    if(iterable != undefined)forOf(iterable, IS_MAP, that[ADDER], that);
  });
  redefineAll(C.prototype, {
    // 23.3.3.2 WeakMap.prototype.delete(key)
    // 23.4.3.3 WeakSet.prototype.delete(value)
    'delete': function(key){
      if(!isObject(key))return false;
      var data = getWeak(key);
      if(data === true)return uncaughtFrozenStore(this)['delete'](key);
      return data && $has(data, this._i) && delete data[this._i];
    },
    // 23.3.3.4 WeakMap.prototype.has(key)
    // 23.4.3.4 WeakSet.prototype.has(value)
    has: function has(key){
      if(!isObject(key))return false;
      var data = getWeak(key);
      if(data === true)return uncaughtFrozenStore(this).has(key);
      return data && $has(data, this._i);
    }
  });
  return C;
}
```
- example usage
```shell
...
	        : function set(a, b){ fn.call(this, a === 0 ? 0 : a, b); return this; }
	    );
	  };
	  if(typeof C != 'function' || !(IS_WEAK || proto.forEach && !fails(function(){
	    new C().entries().next();
	  }))){
	    // create collection constructor
	    C = common.getConstructor(wrapper, NAME, IS_MAP, ADDER);
	    redefineAll(C.prototype, methods);
	    meta.NEED = true;
	  } else {
	    var instance             = new C
	      // early implementations not supports chaining
	      , HASNT_CHAINING       = instance[ADDER](IS_WEAK ? {} : -0, 1) != instance
	      // V8 ~  Chromium 40- weak-collections throws on primitives, but should return false
...
```

#### <a name="apidoc.element.core-js._collection_weak.ufstore"></a>[function <span class="apidocSignatureSpan">core-js._collection_weak.</span>ufstore (that)](#apidoc.element.core-js._collection_weak.ufstore)
- description and source-code
```javascript
ufstore = function (that){
  return that._l || (that._l = new UncaughtFrozenStore);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.core-js._iterators"></a>[module core-js._iterators](#apidoc.module.core-js._iterators)

#### <a name="apidoc.element.core-js._iterators.Arguments"></a>[function <span class="apidocSignatureSpan">core-js._iterators.</span>Arguments ()](#apidoc.element.core-js._iterators.Arguments)
- description and source-code
```javascript
function values() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js._iterators.Array"></a>[function <span class="apidocSignatureSpan">core-js._iterators.</span>Array ()](#apidoc.element.core-js._iterators.Array)
- description and source-code
```javascript
function values() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js._iterators.Float32Array"></a>[function <span class="apidocSignatureSpan">core-js._iterators.</span>Float32Array ()](#apidoc.element.core-js._iterators.Float32Array)
- description and source-code
```javascript
function values() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js._iterators.Float64Array"></a>[function <span class="apidocSignatureSpan">core-js._iterators.</span>Float64Array ()](#apidoc.element.core-js._iterators.Float64Array)
- description and source-code
```javascript
function values() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js._iterators.Int16Array"></a>[function <span class="apidocSignatureSpan">core-js._iterators.</span>Int16Array ()](#apidoc.element.core-js._iterators.Int16Array)
- description and source-code
```javascript
function values() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js._iterators.Int32Array"></a>[function <span class="apidocSignatureSpan">core-js._iterators.</span>Int32Array ()](#apidoc.element.core-js._iterators.Int32Array)
- description and source-code
```javascript
function values() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js._iterators.Int8Array"></a>[function <span class="apidocSignatureSpan">core-js._iterators.</span>Int8Array ()](#apidoc.element.core-js._iterators.Int8Array)
- description and source-code
```javascript
function values() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js._iterators.Map"></a>[function <span class="apidocSignatureSpan">core-js._iterators.</span>Map ()](#apidoc.element.core-js._iterators.Map)
- description and source-code
```javascript
function entries() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js._iterators.Number"></a>[function <span class="apidocSignatureSpan">core-js._iterators.</span>Number ()](#apidoc.element.core-js._iterators.Number)
- description and source-code
```javascript
function entries(){ return new Constructor(this, kind); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js._iterators.Set"></a>[function <span class="apidocSignatureSpan">core-js._iterators.</span>Set ()](#apidoc.element.core-js._iterators.Set)
- description and source-code
```javascript
function values() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js._iterators.String"></a>[function <span class="apidocSignatureSpan">core-js._iterators.</span>String ()](#apidoc.element.core-js._iterators.String)
- description and source-code
```javascript
function [Symbol.iterator]() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js._iterators.Uint16Array"></a>[function <span class="apidocSignatureSpan">core-js._iterators.</span>Uint16Array ()](#apidoc.element.core-js._iterators.Uint16Array)
- description and source-code
```javascript
function values() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js._iterators.Uint32Array"></a>[function <span class="apidocSignatureSpan">core-js._iterators.</span>Uint32Array ()](#apidoc.element.core-js._iterators.Uint32Array)
- description and source-code
```javascript
function values() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js._iterators.Uint8Array"></a>[function <span class="apidocSignatureSpan">core-js._iterators.</span>Uint8Array ()](#apidoc.element.core-js._iterators.Uint8Array)
- description and source-code
```javascript
function values() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js._iterators.Uint8ClampedArray"></a>[function <span class="apidocSignatureSpan">core-js._iterators.</span>Uint8ClampedArray ()](#apidoc.element.core-js._iterators.Uint8ClampedArray)
- description and source-code
```javascript
function values() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.core-js._meta"></a>[module core-js._meta](#apidoc.module.core-js._meta)

#### <a name="apidoc.element.core-js._meta.fastKey"></a>[function <span class="apidocSignatureSpan">core-js._meta.</span>fastKey (it, create)](#apidoc.element.core-js._meta.fastKey)
- description and source-code
```javascript
fastKey = function (it, create){
  // return primitive with prefix
  if(!isObject(it))return typeof it == 'symbol' ? it : (typeof it == 'string' ? 'S' : 'P') + it;
  if(!has(it, META)){
    // can't set metadata to uncaught frozen object
    if(!isExtensible(it))return 'F';
    // not necessary to add metadata
    if(!create)return 'E';
    // add missing metadata
    setMeta(it);
  // return object ID
  } return it[META].i;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js._meta.getWeak"></a>[function <span class="apidocSignatureSpan">core-js._meta.</span>getWeak (it, create)](#apidoc.element.core-js._meta.getWeak)
- description and source-code
```javascript
getWeak = function (it, create){
  if(!has(it, META)){
    // can't set metadata to uncaught frozen object
    if(!isExtensible(it))return true;
    // not necessary to add metadata
    if(!create)return false;
    // add missing metadata
    setMeta(it);
  // return hash weak collections IDs
  } return it[META].w;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js._meta.onFreeze"></a>[function <span class="apidocSignatureSpan">core-js._meta.</span>onFreeze (it)](#apidoc.element.core-js._meta.onFreeze)
- description and source-code
```javascript
onFreeze = function (it){
  if(FREEZE && meta.NEED && isExtensible(it) && !has(it, META))setMeta(it);
  return it;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.core-js._metadata"></a>[module core-js._metadata](#apidoc.module.core-js._metadata)

#### <a name="apidoc.element.core-js._metadata.exp"></a>[function <span class="apidocSignatureSpan">core-js._metadata.</span>exp (O)](#apidoc.element.core-js._metadata.exp)
- description and source-code
```javascript
exp = function (O){
  $export($export.S, 'Reflect', O);
}
```
- example usage
```shell
...
	var $expm1 = Math.expm1;
	module.exports = (!$expm1
	  // Old FF bug
	  || $expm1(10) > 22025.465794806719 || $expm1(10) < 22025.4657948067165168
	  // Tor Browser bug
	  || $expm1(-2e-17) != -2e-17
	) ? function expm1(x){
	  return (x = +x) == 0 ? x : x > -1e-6 && x < 1e-6 ? x + x * x / 2 : Math.exp(x) - 1;
	} : $expm1;

/***/ },
/* 111 */
/***/ function(module, exports, __webpack_require__) {

	// 20.2.2.16 Math.fround(x)
...
```

#### <a name="apidoc.element.core-js._metadata.get"></a>[function <span class="apidocSignatureSpan">core-js._metadata.</span>get (MetadataKey, O, P)](#apidoc.element.core-js._metadata.get)
- description and source-code
```javascript
get = function (MetadataKey, O, P){
  var metadataMap = getOrCreateMetadataMap(O, P, false);
  return metadataMap === undefined ? undefined : metadataMap.get(MetadataKey);
}
```
- example usage
```shell
...
	'use strict';
	var strong = __webpack_require__(204);

	// 23.1 Map Objects
	module.exports = __webpack_require__(205)('Map', function(get){
	  return function Map(){ return get(this, arguments.length > 0 ? arguments[0] : undefined); };
	}, {
	  // 23.1.3.6 Map.prototype.get(key)
	  get: function get(key){
	    var entry = strong.getEntry(this, key);
	    return entry && entry.v;
	  },
	  // 23.1.3.9 Map.prototype.set(key, value)
	  set: function set(key, value){
	    return strong.def(this, key === 0 ? 0 : key, value);
...
```

#### <a name="apidoc.element.core-js._metadata.has"></a>[function <span class="apidocSignatureSpan">core-js._metadata.</span>has (MetadataKey, O, P)](#apidoc.element.core-js._metadata.has)
- description and source-code
```javascript
has = function (MetadataKey, O, P){
  var metadataMap = getOrCreateMetadataMap(O, P, false);
  return metadataMap === undefined ? false : metadataMap.has(MetadataKey);
}
```
- example usage
```shell
...
	          , entry;
	        while(entry = entry ? entry.n : this._f){
	          f(entry.v, entry.k, this);
	          // revert to the last existing entry
	          while(entry && entry.r)entry = entry.p;
	        }
	      },
	      // 23.1.3.7 Map.prototype.has(key)
	      // 23.2.3.7 Set.prototype.has(value)
	      has: function has(key){
	        return !!getEntry(this, key);
	      }
	    });
	    if(DESCRIPTORS)dP(C.prototype, 'size', {
	      get: function(){
...
```

#### <a name="apidoc.element.core-js._metadata.key"></a>[function <span class="apidocSignatureSpan">core-js._metadata.</span>key (it)](#apidoc.element.core-js._metadata.key)
- description and source-code
```javascript
key = function (it){
  return it === undefined || typeof it == 'symbol' ? it : String(it);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js._metadata.keys"></a>[function <span class="apidocSignatureSpan">core-js._metadata.</span>keys (target, targetKey)](#apidoc.element.core-js._metadata.keys)
- description and source-code
```javascript
keys = function (target, targetKey){
  var metadataMap = getOrCreateMetadataMap(target, targetKey, false)
    , keys        = [];
  if(metadataMap)metadataMap.forEach(function(_, key){ keys.push(key); });
  return keys;
}
```
- example usage
```shell
...
	  while(length > index)if(O[key = keys[index++]] === el)return key;
	};

/***/ },
/* 28 */
/***/ function(module, exports, __webpack_require__) {

	// 19.1.2.14 / 15.2.3.14 Object.keys(O)
	var $keys       = __webpack_require__(29)
	  , enumBugKeys = __webpack_require__(39);

	module.exports = Object.keys || function keys(O){
	  return $keys(O, enumBugKeys);
	};
...
```

#### <a name="apidoc.element.core-js._metadata.map"></a>[function <span class="apidocSignatureSpan">core-js._metadata.</span>map (target, targetKey, create)](#apidoc.element.core-js._metadata.map)
- description and source-code
```javascript
map = function (target, targetKey, create){
  var targetMetadata = store.get(target);
  if(!targetMetadata){
    if(!create)return undefined;
    store.set(target, targetMetadata = new Map);
  }
  var keyMetadata = targetMetadata.get(targetKey);
  if(!keyMetadata){
    if(!create)return undefined;
    targetMetadata.set(targetKey, keyMetadata = new Map);
  } return keyMetadata;
}
```
- example usage
```shell
...
/***/ function(module, exports, __webpack_require__) {

	'use strict';
	var $export = __webpack_require__(6)
	  , $map    = __webpack_require__(164)(1);

	$export($export.P + $export.F * !__webpack_require__(160)([].map, true), 'Array', {
	  // 22.1.3.15 / 15.4.4.19 Array.prototype.map(callbackfn [, thisArg])
	  map: function map(callbackfn /* , thisArg */){
	    return $map(this, callbackfn, arguments[1]);
	  }
	});

/***/ },
/* 168 */
...
```

#### <a name="apidoc.element.core-js._metadata.set"></a>[function <span class="apidocSignatureSpan">core-js._metadata.</span>set (MetadataKey, MetadataValue, O, P)](#apidoc.element.core-js._metadata.set)
- description and source-code
```javascript
set = function (MetadataKey, MetadataValue, O, P){
  getOrCreateMetadataMap(O, P, true).set(MetadataKey, MetadataValue);
}
```
- example usage
```shell
...
	  return function Map(){ return get(this, arguments.length > 0 ? arguments[0] : undefined); };
	}, {
	  // 23.1.3.6 Map.prototype.get(key)
	  get: function get(key){
	    var entry = strong.getEntry(this, key);
	    return entry && entry.v;
	  },
	  // 23.1.3.9 Map.prototype.set(key, value)
	  set: function set(key, value){
	    return strong.def(this, key === 0 ? 0 : key, value);
	  }
	}, strong, true);

/***/ },
/* 204 */
...
```



# <a name="apidoc.module.core-js._object_dp"></a>[module core-js._object_dp](#apidoc.module.core-js._object_dp)

#### <a name="apidoc.element.core-js._object_dp.f"></a>[function <span class="apidocSignatureSpan">core-js._object_dp.</span>f ()](#apidoc.element.core-js._object_dp.f)
- description and source-code
```javascript
function defineProperty() { [native code] }
```
- example usage
```shell
...
/***/ },
/* 8 */
/***/ function(module, exports, __webpack_require__) {

	var dP         = __webpack_require__(9)
	  , createDesc = __webpack_require__(15);
	module.exports = __webpack_require__(4) ? function(object, key, value){
	  return dP.f(object, key, createDesc(1, value));
	} : function(object, key, value){
	  object[key] = value;
	  return object;
	};

/***/ },
/* 9 */
...
```



# <a name="apidoc.module.core-js._object_gopd"></a>[module core-js._object_gopd](#apidoc.module.core-js._object_gopd)

#### <a name="apidoc.element.core-js._object_gopd.f"></a>[function <span class="apidocSignatureSpan">core-js._object_gopd.</span>f ()](#apidoc.element.core-js._object_gopd.f)
- description and source-code
```javascript
function getOwnPropertyDescriptor() { [native code] }
```
- example usage
```shell
...
/***/ },
/* 8 */
/***/ function(module, exports, __webpack_require__) {

	var dP         = __webpack_require__(9)
	  , createDesc = __webpack_require__(15);
	module.exports = __webpack_require__(4) ? function(object, key, value){
	  return dP.f(object, key, createDesc(1, value));
	} : function(object, key, value){
	  object[key] = value;
	  return object;
	};

/***/ },
/* 9 */
...
```



# <a name="apidoc.module.core-js._object_gopn"></a>[module core-js._object_gopn](#apidoc.module.core-js._object_gopn)

#### <a name="apidoc.element.core-js._object_gopn.f"></a>[function <span class="apidocSignatureSpan">core-js._object_gopn.</span>f ()](#apidoc.element.core-js._object_gopn.f)
- description and source-code
```javascript
function getOwnPropertyNames() { [native code] }
```
- example usage
```shell
...
/***/ },
/* 8 */
/***/ function(module, exports, __webpack_require__) {

	var dP         = __webpack_require__(9)
	  , createDesc = __webpack_require__(15);
	module.exports = __webpack_require__(4) ? function(object, key, value){
	  return dP.f(object, key, createDesc(1, value));
	} : function(object, key, value){
	  object[key] = value;
	  return object;
	};

/***/ },
/* 9 */
...
```



# <a name="apidoc.module.core-js._object_gopn_ext"></a>[module core-js._object_gopn_ext](#apidoc.module.core-js._object_gopn_ext)

#### <a name="apidoc.element.core-js._object_gopn_ext.f"></a>[function <span class="apidocSignatureSpan">core-js._object_gopn_ext.</span>f (it)](#apidoc.element.core-js._object_gopn_ext.f)
- description and source-code
```javascript
function getOwnPropertyNames(it){
  return windowNames && toString.call(it) == '[object Window]' ? getWindowNames(it) : gOPN(toIObject(it));
}
```
- example usage
```shell
...
/***/ },
/* 8 */
/***/ function(module, exports, __webpack_require__) {

	var dP         = __webpack_require__(9)
	  , createDesc = __webpack_require__(15);
	module.exports = __webpack_require__(4) ? function(object, key, value){
	  return dP.f(object, key, createDesc(1, value));
	} : function(object, key, value){
	  object[key] = value;
	  return object;
	};

/***/ },
/* 9 */
...
```



# <a name="apidoc.module.core-js._object_gops"></a>[module core-js._object_gops](#apidoc.module.core-js._object_gops)

#### <a name="apidoc.element.core-js._object_gops.f"></a>[function <span class="apidocSignatureSpan">core-js._object_gops.</span>f ()](#apidoc.element.core-js._object_gops.f)
- description and source-code
```javascript
function getOwnPropertySymbols() { [native code] }
```
- example usage
```shell
...
/***/ },
/* 8 */
/***/ function(module, exports, __webpack_require__) {

	var dP         = __webpack_require__(9)
	  , createDesc = __webpack_require__(15);
	module.exports = __webpack_require__(4) ? function(object, key, value){
	  return dP.f(object, key, createDesc(1, value));
	} : function(object, key, value){
	  object[key] = value;
	  return object;
	};

/***/ },
/* 9 */
...
```



# <a name="apidoc.module.core-js._object_pie"></a>[module core-js._object_pie](#apidoc.module.core-js._object_pie)

#### <a name="apidoc.element.core-js._object_pie.f"></a>[function <span class="apidocSignatureSpan">core-js._object_pie.</span>f ()](#apidoc.element.core-js._object_pie.f)
- description and source-code
```javascript
function propertyIsEnumerable() { [native code] }
```
- example usage
```shell
...
/***/ },
/* 8 */
/***/ function(module, exports, __webpack_require__) {

	var dP         = __webpack_require__(9)
	  , createDesc = __webpack_require__(15);
	module.exports = __webpack_require__(4) ? function(object, key, value){
	  return dP.f(object, key, createDesc(1, value));
	} : function(object, key, value){
	  object[key] = value;
	  return object;
	};

/***/ },
/* 9 */
...
```



# <a name="apidoc.module.core-js._set_proto"></a>[module core-js._set_proto](#apidoc.module.core-js._set_proto)

#### <a name="apidoc.element.core-js._set_proto.check"></a>[function <span class="apidocSignatureSpan">core-js._set_proto.</span>check (O, proto)](#apidoc.element.core-js._set_proto.check)
- description and source-code
```javascript
check = function (O, proto){
  anObject(O);
  if(!isObject(proto) && proto !== null)throw TypeError(proto + ": can't set as prototype!");
}
```
- example usage
```shell
...

	// 26.1.14 Reflect.setPrototypeOf(target, proto)
	var $export  = __webpack_require__(6)
	  , setProto = __webpack_require__(71);

	if(setProto)$export($export.S, 'Reflect', {
	  setPrototypeOf: function setPrototypeOf(target, proto){
	    setProto.check(target, proto);
	    try {
	      setProto.set(target, proto);
	      return true;
	    } catch(e){
	      return false;
	    }
	  }
...
```

#### <a name="apidoc.element.core-js._set_proto.set"></a>[function <span class="apidocSignatureSpan">core-js._set_proto.</span>set ()](#apidoc.element.core-js._set_proto.set)
- description and source-code
```javascript
function setPrototypeOf() { [native code] }
```
- example usage
```shell
...
	  return function Map(){ return get(this, arguments.length > 0 ? arguments[0] : undefined); };
	}, {
	  // 23.1.3.6 Map.prototype.get(key)
	  get: function get(key){
	    var entry = strong.getEntry(this, key);
	    return entry && entry.v;
	  },
	  // 23.1.3.9 Map.prototype.set(key, value)
	  set: function set(key, value){
	    return strong.def(this, key === 0 ? 0 : key, value);
	  }
	}, strong, true);

/***/ },
/* 204 */
...
```



# <a name="apidoc.module.core-js._string_trim"></a>[module core-js._string_trim](#apidoc.module.core-js._string_trim)

#### <a name="apidoc.element.core-js._string_trim._string_trim"></a>[function <span class="apidocSignatureSpan">core-js.</span>_string_trim (KEY, exec, ALIAS)](#apidoc.element.core-js._string_trim._string_trim)
- description and source-code
```javascript
_string_trim = function (KEY, exec, ALIAS){
  var exp   = {};
  var FORCE = fails(function(){
    return !!spaces[KEY]() || non[KEY]() != non;
  });
  var fn = exp[KEY] = FORCE ? exec(trim) : spaces[KEY];
  if(ALIAS)exp[ALIAS] = fn;
  $export($export.P + $export.F * FORCE, 'String', exp);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js._string_trim.trim"></a>[function <span class="apidocSignatureSpan">core-js._string_trim.</span>trim (string, TYPE)](#apidoc.element.core-js._string_trim.trim)
- description and source-code
```javascript
trim = function (string, TYPE){
  string = String(defined(string));
  if(TYPE & 1)string = string.replace(ltrim, '');
  if(TYPE & 2)string = string.replace(rtrim, '');
  return string;
}
```
- example usage
```shell
...
	  , BROKEN_COF        = cof(__webpack_require__(44)(proto)) == NUMBER
	  , TRIM              = 'trim' in String.prototype;

	// 7.1.3 ToNumber(argument)
	var toNumber = function(argument){
	  var it = toPrimitive(argument, false);
	  if(typeof it == 'string' && it.length > 2){
	    it = TRIM ? it.trim() : $trim(it, 3);
	    var first = it.charCodeAt(0)
	      , third, radix, maxCode;
	    if(first === 43 || first === 45){
	      third = it.charCodeAt(2);
	      if(third === 88 || third === 120)return NaN; // Number('+0x1') should be NaN, old V8 fix
	    } else if(first === 48){
	      switch(it.charCodeAt(1)){
...
```



# <a name="apidoc.module.core-js._task"></a>[module core-js._task](#apidoc.module.core-js._task)

#### <a name="apidoc.element.core-js._task.clear"></a>[function <span class="apidocSignatureSpan">core-js._task.</span>clear (immediate)](#apidoc.element.core-js._task.clear)
- description and source-code
```javascript
clear = function (immediate) {
  if (!immediate) return;

  immediate._onImmediate = null;

  immediateQueue.remove(immediate);

  if (!immediateQueue.head) {
    process._needImmediateCallback = false;
  }
}
```
- example usage
```shell
...
	      that._i = create(null); // index
	      that._f = undefined;    // first entry
	      that._l = undefined;    // last entry
	      that[SIZE] = 0;         // size
	      if(iterable != undefined)forOf(iterable, IS_MAP, that[ADDER], that);
	    });
	    redefineAll(C.prototype, {
	      // 23.1.3.1 Map.prototype.clear()
	      // 23.2.3.2 Set.prototype.clear()
	      clear: function clear(){
	        for(var that = this, data = that._i, entry = that._f; entry; entry = entry.n){
	          entry.r = true;
	          if(entry.p)entry.p = entry.p.n = undefined;
	          delete data[entry.i];
	        }
...
```

#### <a name="apidoc.element.core-js._task.set"></a>[function <span class="apidocSignatureSpan">core-js._task.</span>set (callback, arg1, arg2, arg3)](#apidoc.element.core-js._task.set)
- description and source-code
```javascript
set = function (callback, arg1, arg2, arg3) {
  if (typeof callback !== 'function') {
    throw new TypeError('"callback" argument must be a function');
  }

  var i, args;

  switch (arguments.length) {
    // fast cases
    case 1:
      break;
    case 2:
      args = [arg1];
      break;
    case 3:
      args = [arg1, arg2];
      break;
    default:
      args = [arg1, arg2, arg3];
      for (i = 4; i < arguments.length; i++)
        // extend array dynamically, makes .apply run much faster in v6.0.0
        args[i - 1] = arguments[i];
      break;
  }
  return createImmediate(args, callback);
}
```
- example usage
```shell
...
	  return function Map(){ return get(this, arguments.length > 0 ? arguments[0] : undefined); };
	}, {
	  // 23.1.3.6 Map.prototype.get(key)
	  get: function get(key){
	    var entry = strong.getEntry(this, key);
	    return entry && entry.v;
	  },
	  // 23.1.3.9 Map.prototype.set(key, value)
	  set: function set(key, value){
	    return strong.def(this, key === 0 ? 0 : key, value);
	  }
	}, strong, true);

/***/ },
/* 204 */
...
```



# <a name="apidoc.module.core-js._typed_buffer"></a>[module core-js._typed_buffer](#apidoc.module.core-js._typed_buffer)

#### <a name="apidoc.element.core-js._typed_buffer.ArrayBuffer"></a>[function <span class="apidocSignatureSpan">core-js._typed_buffer.</span>ArrayBuffer ()](#apidoc.element.core-js._typed_buffer.ArrayBuffer)
- description and source-code
```javascript
function ArrayBuffer() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js._typed_buffer.DataView"></a>[function <span class="apidocSignatureSpan">core-js._typed_buffer.</span>DataView ()](#apidoc.element.core-js._typed_buffer.DataView)
- description and source-code
```javascript
function DataView() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.core-js._wks_ext"></a>[module core-js._wks_ext](#apidoc.module.core-js._wks_ext)

#### <a name="apidoc.element.core-js._wks_ext.f"></a>[function <span class="apidocSignatureSpan">core-js._wks_ext.</span>f (name)](#apidoc.element.core-js._wks_ext.f)
- description and source-code
```javascript
f = function (name){
  return store[name] || (store[name] =
    USE_SYMBOL && Symbol[name] || (USE_SYMBOL ? Symbol : uid)('Symbol.' + name));
}
```
- example usage
```shell
...
/***/ },
/* 8 */
/***/ function(module, exports, __webpack_require__) {

	var dP         = __webpack_require__(9)
	  , createDesc = __webpack_require__(15);
	module.exports = __webpack_require__(4) ? function(object, key, value){
	  return dP.f(object, key, createDesc(1, value));
	} : function(object, key, value){
	  object[key] = value;
	  return object;
	};

/***/ },
/* 9 */
...
```



# <a name="apidoc.module.core-js.core"></a>[module core-js.core](#apidoc.module.core-js.core)

#### <a name="apidoc.element.core-js.core.getIterator"></a>[function <span class="apidocSignatureSpan">core-js.core.</span>getIterator (it)](#apidoc.element.core-js.core.getIterator)
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

#### <a name="apidoc.element.core-js.core.getIteratorMethod"></a>[function <span class="apidocSignatureSpan">core-js.core.</span>getIteratorMethod (it)](#apidoc.element.core-js.core.getIteratorMethod)
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

#### <a name="apidoc.element.core-js.core.inspectSource"></a>[function <span class="apidocSignatureSpan">core-js.core.</span>inspectSource (it)](#apidoc.element.core-js.core.inspectSource)
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

#### <a name="apidoc.element.core-js.core.isIterable"></a>[function <span class="apidocSignatureSpan">core-js.core.</span>isIterable (it)](#apidoc.element.core-js.core.isIterable)
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



# <a name="apidoc.module.core-js.es6_array_iterator"></a>[module core-js.es6_array_iterator](#apidoc.module.core-js.es6_array_iterator)

#### <a name="apidoc.element.core-js.es6_array_iterator.entries"></a>[function <span class="apidocSignatureSpan">core-js.es6_array_iterator.</span>entries ()](#apidoc.element.core-js.es6_array_iterator.entries)
- description and source-code
```javascript
function entries() { [native code] }
```
- example usage
```shell
...

	'use strict';
	var addToUnscopables = __webpack_require__(178)
	  , step             = __webpack_require__(184)
	  , Iterators        = __webpack_require__(135)
	  , toIObject        = __webpack_require__(30);

	// 22.1.3.4 Array.prototype.entries()
	// 22.1.3.13 Array.prototype.keys()
	// 22.1.3.29 Array.prototype.values()
	// 22.1.3.30 Array.prototype[@@iterator]()
	module.exports = __webpack_require__(134)(Array, 'Array', function(iterated, kind){
	  this._t = toIObject(iterated); // target
	  this._i = 0;                   // next index
	  this._k = kind;                // kind
...
```

#### <a name="apidoc.element.core-js.es6_array_iterator.keys"></a>[function <span class="apidocSignatureSpan">core-js.es6_array_iterator.</span>keys ()](#apidoc.element.core-js.es6_array_iterator.keys)
- description and source-code
```javascript
function keys() { [native code] }
```
- example usage
```shell
...
	  while(length > index)if(O[key = keys[index++]] === el)return key;
	};

/***/ },
/* 28 */
/***/ function(module, exports, __webpack_require__) {

	// 19.1.2.14 / 15.2.3.14 Object.keys(O)
	var $keys       = __webpack_require__(29)
	  , enumBugKeys = __webpack_require__(39);

	module.exports = Object.keys || function keys(O){
	  return $keys(O, enumBugKeys);
	};
...
```

#### <a name="apidoc.element.core-js.es6_array_iterator.values"></a>[function <span class="apidocSignatureSpan">core-js.es6_array_iterator.</span>values ()](#apidoc.element.core-js.es6_array_iterator.values)
- description and source-code
```javascript
function values() { [native code] }
```
- example usage
```shell
...
	var addToUnscopables = __webpack_require__(178)
	  , step             = __webpack_require__(184)
	  , Iterators        = __webpack_require__(135)
	  , toIObject        = __webpack_require__(30);

	// 22.1.3.4 Array.prototype.entries()
	// 22.1.3.13 Array.prototype.keys()
	// 22.1.3.29 Array.prototype.values()
	// 22.1.3.30 Array.prototype[@@iterator]()
	module.exports = __webpack_require__(134)(Array, 'Array', function(iterated, kind){
	  this._t = toIObject(iterated); // target
	  this._i = 0;                   // next index
	  this._k = kind;                // kind
	// 22.1.5.2.1 %ArrayIteratorPrototype%.next()
	}, function(){
...
```



# <a name="apidoc.module.core-js.library"></a>[module core-js.library](#apidoc.module.core-js.library)

#### <a name="apidoc.element.core-js.library.ArrayBuffer"></a>[function <span class="apidocSignatureSpan">core-js.library.</span>ArrayBuffer (a, b, c)](#apidoc.element.core-js.library.ArrayBuffer)
- description and source-code
```javascript
ArrayBuffer = function (a, b, c){
	        if(this instanceof C){
	          switch(arguments.length){
	            case 0: return new C;
	            case 1: return new C(a);
	            case 2: return new C(a, b);
	          } return new C(a, b, c);
	        } return C.apply(this, arguments);
	      }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.library.DataView"></a>[function <span class="apidocSignatureSpan">core-js.library.</span>DataView (a, b, c)](#apidoc.element.core-js.library.DataView)
- description and source-code
```javascript
DataView = function (a, b, c){
	        if(this instanceof C){
	          switch(arguments.length){
	            case 0: return new C;
	            case 1: return new C(a);
	            case 2: return new C(a, b);
	          } return new C(a, b, c);
	        } return C.apply(this, arguments);
	      }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.library.Dict"></a>[function <span class="apidocSignatureSpan">core-js.library.</span>Dict (iterable)](#apidoc.element.core-js.library.Dict)
- description and source-code
```javascript
function Dict(iterable){
	  var dict = create(null);
	  if(iterable != undefined){
	    if(isIterable(iterable)){
	      forOf(iterable, true, function(key, value){
	        dict[key] = value;
	      });
	    } else assign(dict, iterable);
	  }
	  return dict;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.library.Float32Array"></a>[function <span class="apidocSignatureSpan">core-js.library.</span>Float32Array (a, b, c)](#apidoc.element.core-js.library.Float32Array)
- description and source-code
```javascript
Float32Array = function (a, b, c){
	        if(this instanceof C){
	          switch(arguments.length){
	            case 0: return new C;
	            case 1: return new C(a);
	            case 2: return new C(a, b);
	          } return new C(a, b, c);
	        } return C.apply(this, arguments);
	      }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.library.Float64Array"></a>[function <span class="apidocSignatureSpan">core-js.library.</span>Float64Array (a, b, c)](#apidoc.element.core-js.library.Float64Array)
- description and source-code
```javascript
Float64Array = function (a, b, c){
	        if(this instanceof C){
	          switch(arguments.length){
	            case 0: return new C;
	            case 1: return new C(a);
	            case 2: return new C(a, b);
	          } return new C(a, b, c);
	        } return C.apply(this, arguments);
	      }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.library.Int16Array"></a>[function <span class="apidocSignatureSpan">core-js.library.</span>Int16Array (a, b, c)](#apidoc.element.core-js.library.Int16Array)
- description and source-code
```javascript
Int16Array = function (a, b, c){
	        if(this instanceof C){
	          switch(arguments.length){
	            case 0: return new C;
	            case 1: return new C(a);
	            case 2: return new C(a, b);
	          } return new C(a, b, c);
	        } return C.apply(this, arguments);
	      }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.library.Int32Array"></a>[function <span class="apidocSignatureSpan">core-js.library.</span>Int32Array (a, b, c)](#apidoc.element.core-js.library.Int32Array)
- description and source-code
```javascript
Int32Array = function (a, b, c){
	        if(this instanceof C){
	          switch(arguments.length){
	            case 0: return new C;
	            case 1: return new C(a);
	            case 2: return new C(a, b);
	          } return new C(a, b, c);
	        } return C.apply(this, arguments);
	      }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.library.Int8Array"></a>[function <span class="apidocSignatureSpan">core-js.library.</span>Int8Array (a, b, c)](#apidoc.element.core-js.library.Int8Array)
- description and source-code
```javascript
Int8Array = function (a, b, c){
	        if(this instanceof C){
	          switch(arguments.length){
	            case 0: return new C;
	            case 1: return new C(a);
	            case 2: return new C(a, b);
	          } return new C(a, b, c);
	        } return C.apply(this, arguments);
	      }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.library.Map"></a>[function <span class="apidocSignatureSpan">core-js.library.</span>Map ()](#apidoc.element.core-js.library.Map)
- description and source-code
```javascript
function Map(){ return get(this, arguments.length > 0 ? arguments[0] : undefined); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.library.Observable"></a>[function <span class="apidocSignatureSpan">core-js.library.</span>Observable ()](#apidoc.element.core-js.library.Observable)
- description and source-code
```javascript
function Observable() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.library.Promise"></a>[function <span class="apidocSignatureSpan">core-js.library.</span>Promise (a, b, c)](#apidoc.element.core-js.library.Promise)
- description and source-code
```javascript
Promise = function (a, b, c){
	        if(this instanceof C){
	          switch(arguments.length){
	            case 0: return new C;
	            case 1: return new C(a);
	            case 2: return new C(a, b);
	          } return new C(a, b, c);
	        } return C.apply(this, arguments);
	      }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.library.Set"></a>[function <span class="apidocSignatureSpan">core-js.library.</span>Set ()](#apidoc.element.core-js.library.Set)
- description and source-code
```javascript
function Set(){ return get(this, arguments.length > 0 ? arguments[0] : undefined); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.library.Symbol"></a>[function <span class="apidocSignatureSpan">core-js.library.</span>Symbol (a, b, c)](#apidoc.element.core-js.library.Symbol)
- description and source-code
```javascript
Symbol = function (a, b, c){
	        if(this instanceof C){
	          switch(arguments.length){
	            case 0: return new C;
	            case 1: return new C(a);
	            case 2: return new C(a, b);
	          } return new C(a, b, c);
	        } return C.apply(this, arguments);
	      }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.library.Uint16Array"></a>[function <span class="apidocSignatureSpan">core-js.library.</span>Uint16Array (a, b, c)](#apidoc.element.core-js.library.Uint16Array)
- description and source-code
```javascript
Uint16Array = function (a, b, c){
	        if(this instanceof C){
	          switch(arguments.length){
	            case 0: return new C;
	            case 1: return new C(a);
	            case 2: return new C(a, b);
	          } return new C(a, b, c);
	        } return C.apply(this, arguments);
	      }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.library.Uint32Array"></a>[function <span class="apidocSignatureSpan">core-js.library.</span>Uint32Array (a, b, c)](#apidoc.element.core-js.library.Uint32Array)
- description and source-code
```javascript
Uint32Array = function (a, b, c){
	        if(this instanceof C){
	          switch(arguments.length){
	            case 0: return new C;
	            case 1: return new C(a);
	            case 2: return new C(a, b);
	          } return new C(a, b, c);
	        } return C.apply(this, arguments);
	      }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.library.Uint8Array"></a>[function <span class="apidocSignatureSpan">core-js.library.</span>Uint8Array (a, b, c)](#apidoc.element.core-js.library.Uint8Array)
- description and source-code
```javascript
Uint8Array = function (a, b, c){
	        if(this instanceof C){
	          switch(arguments.length){
	            case 0: return new C;
	            case 1: return new C(a);
	            case 2: return new C(a, b);
	          } return new C(a, b, c);
	        } return C.apply(this, arguments);
	      }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.library.Uint8ClampedArray"></a>[function <span class="apidocSignatureSpan">core-js.library.</span>Uint8ClampedArray (a, b, c)](#apidoc.element.core-js.library.Uint8ClampedArray)
- description and source-code
```javascript
Uint8ClampedArray = function (a, b, c){
	        if(this instanceof C){
	          switch(arguments.length){
	            case 0: return new C;
	            case 1: return new C(a);
	            case 2: return new C(a, b);
	          } return new C(a, b, c);
	        } return C.apply(this, arguments);
	      }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.library.WeakMap"></a>[function <span class="apidocSignatureSpan">core-js.library.</span>WeakMap ()](#apidoc.element.core-js.library.WeakMap)
- description and source-code
```javascript
function WeakMap(){
	    return get(this, arguments.length > 0 ? arguments[0] : undefined);
	  }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.library.WeakSet"></a>[function <span class="apidocSignatureSpan">core-js.library.</span>WeakSet ()](#apidoc.element.core-js.library.WeakSet)
- description and source-code
```javascript
function WeakSet(){ return get(this, arguments.length > 0 ? arguments[0] : undefined); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.library.asap"></a>[function <span class="apidocSignatureSpan">core-js.library.</span>asap ()](#apidoc.element.core-js.library.asap)
- description and source-code
```javascript
function asap() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.library.clearImmediate"></a>[function <span class="apidocSignatureSpan">core-js.library.</span>clearImmediate ()](#apidoc.element.core-js.library.clearImmediate)
- description and source-code
```javascript
clearImmediate = function (){
	    return fn.apply(that, arguments);
	  }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.library.delay"></a>[function <span class="apidocSignatureSpan">core-js.library.</span>delay (time)](#apidoc.element.core-js.library.delay)
- description and source-code
```javascript
function delay(time){
	    return new (core.Promise || global.Promise)(function(resolve){
	      setTimeout(partial.call(resolve, true), time);
	    });
	  }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.library.getIterator"></a>[function <span class="apidocSignatureSpan">core-js.library.</span>getIterator (it)](#apidoc.element.core-js.library.getIterator)
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

#### <a name="apidoc.element.core-js.library.getIteratorMethod"></a>[function <span class="apidocSignatureSpan">core-js.library.</span>getIteratorMethod (it)](#apidoc.element.core-js.library.getIteratorMethod)
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

#### <a name="apidoc.element.core-js.library.isIterable"></a>[function <span class="apidocSignatureSpan">core-js.library.</span>isIterable (it)](#apidoc.element.core-js.library.isIterable)
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

#### <a name="apidoc.element.core-js.library.parseFloat"></a>[function <span class="apidocSignatureSpan">core-js.library.</span>parseFloat ()](#apidoc.element.core-js.library.parseFloat)
- description and source-code
```javascript
function parseFloat() { [native code] }
```
- example usage
```shell
...

/***/ },
/* 95 */
/***/ function(module, exports, __webpack_require__) {

	var $export     = __webpack_require__(6)
	  , $parseFloat = __webpack_require__(96);
	// 20.1.2.12 Number.parseFloat(string)
	$export($export.S + $export.F * (Number.parseFloat != $parseFloat), 'Number', {parseFloat: $parseFloat});

/***/ },
/* 96 */
/***/ function(module, exports, __webpack_require__) {

	var $parseFloat = __webpack_require__(2).parseFloat
...
```

#### <a name="apidoc.element.core-js.library.parseInt"></a>[function <span class="apidocSignatureSpan">core-js.library.</span>parseInt ()](#apidoc.element.core-js.library.parseInt)
- description and source-code
```javascript
function parseInt() { [native code] }
```
- example usage
```shell
...

/***/ },
/* 97 */
/***/ function(module, exports, __webpack_require__) {

	var $export   = __webpack_require__(6)
	  , $parseInt = __webpack_require__(98);
	// 20.1.2.13 Number.parseInt(string, radix)
	$export($export.S + $export.F * (Number.parseInt != $parseInt), 'Number', {parseInt: $parseInt});

/***/ },
/* 98 */
/***/ function(module, exports, __webpack_require__) {

	var $parseInt = __webpack_require__(2).parseInt
...
```

#### <a name="apidoc.element.core-js.library.setImmediate"></a>[function <span class="apidocSignatureSpan">core-js.library.</span>setImmediate ()](#apidoc.element.core-js.library.setImmediate)
- description and source-code
```javascript
setImmediate = function (){
	    return fn.apply(that, arguments);
	  }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.library.setInterval"></a>[function <span class="apidocSignatureSpan">core-js.library.</span>setInterval ()](#apidoc.element.core-js.library.setInterval)
- description and source-code
```javascript
setInterval = function (){
	    return fn.apply(that, arguments);
	  }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.core-js.library.setTimeout"></a>[function <span class="apidocSignatureSpan">core-js.library.</span>setTimeout ()](#apidoc.element.core-js.library.setTimeout)
- description and source-code
```javascript
setTimeout = function (){
	    return fn.apply(that, arguments);
	  }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.core-js.shim"></a>[module core-js.shim](#apidoc.module.core-js.shim)

#### <a name="apidoc.element.core-js.shim.getIteratorMethod"></a>[function <span class="apidocSignatureSpan">core-js.shim.</span>getIteratorMethod (it)](#apidoc.element.core-js.shim.getIteratorMethod)
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

#### <a name="apidoc.element.core-js.shim.inspectSource"></a>[function <span class="apidocSignatureSpan">core-js.shim.</span>inspectSource (it)](#apidoc.element.core-js.shim.inspectSource)
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



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
