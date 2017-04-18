# npmtest-axios

#### test coverage for  [axios (v0.16.1)](https://github.com/mzabriskie/axios)  [![npm package](https://img.shields.io/npm/v/npmtest-axios.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-axios) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-axios.svg)](https://travis-ci.org/npmtest/node-npmtest-axios)

#### Promise based HTTP client for the browser and node.js

[![NPM](https://nodei.co/npm/axios.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/axios)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-axios/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-axios/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-axios/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-axios/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-axios/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-axios/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-axios/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-axios/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-axios/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-axios/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-axios/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-axios/build/test-report.html](https://npmtest.github.io/node-npmtest-axios/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-axios/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-axios/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-axios/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-axios/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-axios/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-axios/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-axios/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-axios/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Matt Zabriskie"
    },
    "browser": {
        "./lib/adapters/http.js": "./lib/adapters/xhr.js"
    },
    "bugs": {
        "url": "https://github.com/mzabriskie/axios/issues"
    },
    "dependencies": {
        "follow-redirects": "^1.2.3"
    },
    "description": "Promise based HTTP client for the browser and node.js",
    "devDependencies": {
        "coveralls": "^2.11.9",
        "es6-promise": "^4.0.5",
        "grunt": "^1.0.1",
        "grunt-banner": "^0.6.0",
        "grunt-cli": "^1.2.0",
        "grunt-contrib-clean": "^1.0.0",
        "grunt-contrib-nodeunit": "^1.0.0",
        "grunt-contrib-watch": "^1.0.0",
        "grunt-eslint": "^19.0.0",
        "grunt-karma": "^2.0.0",
        "grunt-ts": "^6.0.0-beta.3",
        "grunt-webpack": "^1.0.18",
        "istanbul-instrumenter-loader": "^1.0.0",
        "jasmine-core": "^2.4.1",
        "karma": "^1.3.0",
        "karma-chrome-launcher": "^2.0.0",
        "karma-coverage": "^1.0.0",
        "karma-firefox-launcher": "^1.0.0",
        "karma-jasmine": "^1.0.2",
        "karma-jasmine-ajax": "^0.1.13",
        "karma-opera-launcher": "^1.0.0",
        "karma-phantomjs-launcher": "^1.0.0",
        "karma-safari-launcher": "^1.0.0",
        "karma-sauce-launcher": "^1.1.0",
        "karma-sinon": "^1.0.5",
        "karma-sourcemap-loader": "^0.3.7",
        "karma-webpack": "^1.7.0",
        "load-grunt-tasks": "^3.5.2",
        "minimist": "^1.2.0",
        "phantomjs-prebuilt": "^2.1.7",
        "sinon": "^1.17.4",
        "typescript": "^2.0.3",
        "url-search-params": "^0.6.1",
        "webpack": "^1.13.1",
        "webpack-dev-server": "^1.14.1"
    },
    "directories": {},
    "dist": {
        "shasum": "c0b6d26600842384b8f509e57111f0d2df8223ca",
        "tarball": "https://registry.npmjs.org/axios/-/axios-0.16.1.tgz"
    },
    "gitHead": "5c8095e48329dacaec1f8d43a9b84ed275fbd0ef",
    "homepage": "https://github.com/mzabriskie/axios",
    "keywords": [
        "xhr",
        "http",
        "ajax",
        "promise",
        "node"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "mzabriskie"
        },
        {
            "name": "nickuraltsev"
        }
    ],
    "name": "axios",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/mzabriskie/axios.git"
    },
    "scripts": {
        "build": "NODE_ENV=production grunt build",
        "coveralls": "cat coverage/lcov.info | ./node_modules/coveralls/bin/coveralls.js",
        "examples": "node ./examples/server.js",
        "postversion": "git push && git push --tags",
        "preversion": "npm test",
        "start": "node ./sandbox/server.js",
        "test": "grunt test",
        "version": "npm run build && grunt version && git add -A dist && git add CHANGELOG.md bower.json package.json"
    },
    "typings": "./index.d.ts",
    "version": "0.16.1"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
