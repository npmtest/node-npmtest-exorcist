# npmtest-exorcist

#### basic test coverage for  [exorcist (v0.4.0)](https://github.com/thlorenz/exorcist)  [![npm package](https://img.shields.io/npm/v/npmtest-exorcist.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-exorcist) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-exorcist.svg)](https://travis-ci.org/npmtest/node-npmtest-exorcist)

#### Externalizes the source map found inside a stream to an external `.js.map` file

[![NPM](https://nodei.co/npm/exorcist.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/exorcist)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-exorcist/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-exorcist/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-exorcist/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-exorcist/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-exorcist/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-exorcist/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-exorcist/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-exorcist/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-exorcist/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-exorcist/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-exorcist/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-exorcist/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-exorcist/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-exorcist/build/test-report.html](https://npmtest.github.io/node-npmtest-exorcist/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-exorcist/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-exorcist/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-exorcist/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-exorcist/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-exorcist/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-exorcist/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-exorcist/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-exorcist/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Thorsten Lorenz",
        "url": "http://thlorenz.com"
    },
    "bin": {
        "exorcist": "./bin/exorcist.js"
    },
    "bugs": {
        "url": "https://github.com/thlorenz/exorcist/issues"
    },
    "dependencies": {
        "minimist": "0.0.5",
        "mold-source-map": "~0.4.0",
        "nave": "~0.5.1"
    },
    "description": "Externalizes the source map found inside a stream to an external '.js.map' file",
    "devDependencies": {
        "browserify": "~10.2.0",
        "tap": "~0.4.3",
        "through2": "~0.4.0"
    },
    "directories": {},
    "dist": {
        "shasum": "1230ffdedd9248f42fbccf8b4a44d4cab29e3c64",
        "tarball": "https://registry.npmjs.org/exorcist/-/exorcist-0.4.0.tgz"
    },
    "engine": {
        "node": ">=0.6"
    },
    "gitHead": "2ea417707404f3b612b6ffbbbd3ba88e7393af17",
    "homepage": "https://github.com/thlorenz/exorcist",
    "keywords": [
        "source-map",
        "source",
        "map",
        "external",
        "mapfile",
        "browserify",
        "browserify-tool"
    ],
    "license": {
        "type": "MIT",
        "url": "https://github.com/thlorenz/exorcist/blob/master/LICENSE"
    },
    "main": "index.js",
    "maintainers": [
        {
            "name": "thlorenz"
        }
    ],
    "name": "exorcist",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/thlorenz/exorcist.git"
    },
    "scripts": {
        "test": "if [ -e $TRAVIS ]; then npm run test-all; else npm run test-main; fi",
        "test-0.10": " nave use 0.10 npm run test-main",
        "test-0.12": " nave use 0.12 npm run test-main",
        "test-all": "npm run test-main && npm run test-0.10 && npm run test-0.12 && npm run test-iojs",
        "test-iojs": " nave use latest npm run test-main",
        "test-main": "tap test/*.js"
    },
    "version": "0.4.0"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
