# npmtest-tmi.js

#### basic test coverage for  [tmi.js (v1.2.0)](https://github.com/tmijs/tmi.js#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-tmi.js.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-tmi.js) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-tmi.js.svg)](https://travis-ci.org/npmtest/node-npmtest-tmi.js)

#### Javascript library for the Twitch Messaging Interface.

[![NPM](https://nodei.co/npm/tmi.js.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/tmi.js)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-tmi.js/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-tmi.js/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-tmi.js/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-tmi.js/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-tmi.js/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-tmi.js/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-tmi.js/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-tmi.js/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-tmi.js/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-tmi.js/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-tmi.js/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-tmi.js/build/test-report.html](https://npmtest.github.io/node-npmtest-tmi.js/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-tmi.js/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-tmi.js/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-tmi.js/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-tmi.js/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-tmi.js/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-tmi.js/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-tmi.js/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-tmi.js/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Schmoopiie"
    },
    "browser": {
        "ws": false,
        "request": false
    },
    "browserify": {
        "transform": [
            [
                "babelify",
                {
                    "presets": [
                        "es2015"
                    ]
                }
            ]
        ]
    },
    "bugs": {
        "url": "https://github.com/tmijs/tmi.js/issues"
    },
    "contributors": [
        {
            "name": "celluj34"
        }
    ],
    "dependencies": {
        "request": "2.74.0",
        "ws": "1.0.1"
    },
    "description": "Javascript library for the Twitch Messaging Interface.",
    "devDependencies": {
        "babel-preset-es2015": "6.6.0",
        "babelify": "7.2.0",
        "browserify": "13.0.0",
        "hook-std": "0.2.0",
        "istanbul": "0.4.2",
        "mkdirp": "0.5.1",
        "mocha": "2.2.5",
        "npm-run-all": "1.7.0",
        "rimraf": "2.5.2",
        "should": "7.0.4",
        "uglify-js": "2.6.2"
    },
    "directories": {},
    "dist": {
        "shasum": "7e48e48a09d4faa4238d3e417d2ce87fe8287ebd",
        "tarball": "https://registry.npmjs.org/tmi.js/-/tmi.js-1.2.0.tgz"
    },
    "engines": {
        "node": ">=4.4.0"
    },
    "files": [
        "lib",
        "index.js",
        "LICENSE"
    ],
    "gitHead": "84957dfd96d12eb927f06afe25209efd7263b8a1",
    "homepage": "https://github.com/tmijs/tmi.js#readme",
    "keywords": [
        "tmi",
        "twitch",
        "twitch.tv",
        "stream",
        "broadcast",
        "message",
        "messaging",
        "interface",
        "subscriber",
        "websocket",
        "ws",
        "bot",
        "robot"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "schmoopiie"
        }
    ],
    "name": "tmi.js",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/tmijs/tmi.js.git"
    },
    "scripts": {
        "build": "npm-run-all --sequential build:*",
        "build:browserify": "browserify index.js -o ./build/tmi.js",
        "build:dedupe": "npm dedupe",
        "build:mkdirp": "mkdirp ./build",
        "build:rimraf": "rimraf ./build",
        "build:sri": "node sri.js ./build/tmi.js",
        "build:sri-min": "node sri.js ./build/tmi.min.js",
        "build:uglify": "uglifyjs --compress --mangle --output ./build/tmi.min.js --source-map ./build/tmi.js.map ./build/tmi.js",
        "test": "istanbul cover node_modules/mocha/bin/_mocha -- -R spec --require should"
    },
    "version": "1.2.0",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
