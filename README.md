# npmdoc-tween.js

#### api documentation for  [tween.js (v16.6.0)](https://github.com/tweenjs/tween.js)  [![npm package](https://img.shields.io/npm/v/npmdoc-tween.js.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-tween.js) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-tween.js.svg)](https://travis-ci.org/npmdoc/node-npmdoc-tween.js)

#### Super simple, fast and easy to use tweening engine which incorporates optimised Robert Penner's equations.

[![NPM](https://nodei.co/npm/tween.js.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/tween.js)

- [https://npmdoc.github.io/node-npmdoc-tween.js/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-tween.js/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-tween.js/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-tween.js/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-tween.js/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-tween.js/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "tween.js contributors",
        "url": "https://github.com/tweenjs/tween.js/graphs/contributors"
    },
    "bugs": {
        "url": "https://github.com/tweenjs/tween.js/issues"
    },
    "dependencies": {},
    "description": "Super simple, fast and easy to use tweening engine which incorporates optimised Robert Penner's equations.",
    "devDependencies": {
        "jscs": "^2.2.0",
        "jshint": "^2.8.0",
        "nodeunit": "^0.9.1",
        "semantic-release": "^6.3.2"
    },
    "directories": {},
    "dist": {
        "shasum": "739104c9336cc4f11ee53f9ce7cede51e6723624",
        "tarball": "https://registry.npmjs.org/tween.js/-/tween.js-16.6.0.tgz"
    },
    "gitHead": "ae085330fbc0c4e7911c69e786bd3f697f95943f",
    "homepage": "https://github.com/tweenjs/tween.js",
    "keywords": [
        "tween",
        "interpolation"
    ],
    "license": "MIT",
    "main": "src/Tween.js",
    "maintainers": [
        {
            "name": "sole"
        }
    ],
    "name": "tween.js",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/tweenjs/tween.js.git"
    },
    "scripts": {
        "semantic-release": "semantic-release pre && npm publish && semantic-release post",
        "test": "npm run test-unit && npm run test-correctness && npm run test-style",
        "test-correctness": "jshint --config test/jshintrc src/Tween.js",
        "test-style": "jscs --config test/jscs.json src/Tween.js",
        "test-unit": "nodeunit test/unit/nodeunitheadless.js"
    },
    "version": "16.6.0"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
