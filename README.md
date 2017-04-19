# npmdoc-raf

#### api documentation for  [raf (v3.3.0)](https://github.com/chrisdickinson/raf#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-raf.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-raf) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-raf.svg)](https://travis-ci.org/npmdoc/node-npmdoc-raf)

#### requestAnimationFrame polyfill for node and the browser

[![NPM](https://nodei.co/npm/raf.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/raf)

- [https://npmdoc.github.io/node-npmdoc-raf/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-raf/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-raf/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-raf/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-raf/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-raf/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Chris Dickinson"
    },
    "bugs": {
        "url": "https://github.com/chrisdickinson/raf/issues"
    },
    "contributors": [
        {
            "name": "Christian Maughan Tegnér"
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
            "name": "chrisdickinson"
        },
        {
            "name": "cmtegner"
        }
    ],
    "name": "raf",
    "optionalDependencies": {},
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



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
