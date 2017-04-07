# api documentation for  [raf (v3.3.0)](https://github.com/chrisdickinson/raf#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-raf.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-raf) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-raf.svg)](https://travis-ci.org/npmdoc/node-npmdoc-raf)
#### requestAnimationFrame polyfill for node and the browser

[![NPM](https://nodei.co/npm/raf.png?downloads=true)](https://www.npmjs.com/package/raf)

[![apidoc](https://npmdoc.github.io/node-npmdoc-raf/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-raf_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-raf/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-raf/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-raf/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Chris Dickinson",
        "email": "chris@neversaw.us"
    },
    "bugs": {
        "url": "https://github.com/chrisdickinson/raf/issues"
    },
    "contributors": [
        {
            "name": "Christian Maughan Tegnér",
            "email": "christian.tegner@gmail.com"
        }
    ],
    "dependencies": {
        "performance-now": "~0.2.0"
    },
    "description": "requestAnimationFrame polyfill for node and the browser",
    "devDependencies": {
        "browserify": "~4.1.2",
        "tape": "^4.0.0",
        "testling": "~1.6.1"
    },
    "directories": {},
    "dist": {
        "shasum": "93845eeffc773f8129039f677f80a36044eee2c3",
        "tarball": "https://registry.npmjs.org/raf/-/raf-3.3.0.tgz"
    },
    "gitHead": "77781df73108fe4e28599ec72f4975820ed2ecaa",
    "homepage": "https://github.com/chrisdickinson/raf#readme",
    "keywords": [
        "requestAnimationFrame",
        "polyfill"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "chrisdickinson",
            "email": "chris@neversaw.us"
        },
        {
            "name": "cmtegner",
            "email": "christian.tegner@gmail.com"
        }
    ],
    "name": "raf",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/chrisdickinson/raf.git"
    },
    "scripts": {
        "test": "node test.js",
        "testling": "browserify test.js | testling"
    },
    "testling": {
        "files": "test.js",
        "browsers": [
            "iexplore/6.0..latest",
            "firefox/3.0..6.0",
            "firefox/15.0..latest",
            "firefox/nightly",
            "chrome/4.0..10.0",
            "chrome/20.0..latest",
            "chrome/canary",
            "opera/10.0..latest",
            "opera/next",
            "safari/4.0..latest",
            "ipad/6.0..latest",
            "iphone/6.0..latest"
        ]
    },
    "version": "3.3.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module raf](#apidoc.module.raf)
1.  [function <span class="apidocSignatureSpan">raf.</span>cancel ()](#apidoc.element.raf.cancel)
1.  [function <span class="apidocSignatureSpan">raf.</span>polyfill ()](#apidoc.element.raf.polyfill)



# <a name="apidoc.module.raf"></a>[module raf](#apidoc.module.raf)

#### <a name="apidoc.element.raf.cancel"></a>[function <span class="apidocSignatureSpan">raf.</span>cancel ()](#apidoc.element.raf.cancel)
- description and source-code
```javascript
cancel = function () {
  caf.apply(root, arguments)
}
```
- example usage
```shell
...
var raf = require('raf')
'''

## var handle = raf(callback)

'callback' is the function to invoke in the next frame. 'handle' is a long integer value that uniquely identifies the entry in the
 callback list. This is a non-zero value, but you may not make any other assumptions about its value.

## raf.cancel(handle)

'handle' is the entry identifier returned by 'raf()'. Removes the queued animation frame callback (other queued callbacks will still
 be invoked unless cancelled).

## raf.polyfill()

Shorthand to polyfill 'window.requestAnimationFrame' and 'window.cancelAnimationFrame' if necessary (Polyfills 'global' in node).
...
```

#### <a name="apidoc.element.raf.polyfill"></a>[function <span class="apidocSignatureSpan">raf.</span>polyfill ()](#apidoc.element.raf.polyfill)
- description and source-code
```javascript
polyfill = function () {
  root.requestAnimationFrame = raf
  root.cancelAnimationFrame = caf
}
```
- example usage
```shell
...

'callback' is the function to invoke in the next frame. 'handle' is a long integer value that uniquely identifies the entry in the
 callback list. This is a non-zero value, but you may not make any other assumptions about its value.

## raf.cancel(handle)

'handle' is the entry identifier returned by 'raf()'. Removes the queued animation frame callback (other queued callbacks will still
 be invoked unless cancelled).

## raf.polyfill()

Shorthand to polyfill 'window.requestAnimationFrame' and 'window.cancelAnimationFrame' if necessary (Polyfills 'global' in node).

Alternatively you can require 'raf/polyfill' which will act the same as 'require('raf').polyfill()'.

# Acknowledgments
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
