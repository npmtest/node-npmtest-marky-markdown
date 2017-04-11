# test coverage for  [marky-markdown (v9.0.2)](https://github.com/npm/marky-markdown)  [![npm package](https://img.shields.io/npm/v/npmtest-marky-markdown.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-marky-markdown) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-marky-markdown.svg)](https://travis-ci.org/npmtest/node-npmtest-marky-markdown)
#### npm's markdown parser

[![NPM](https://nodei.co/npm/marky-markdown.png?downloads=true)](https://www.npmjs.com/package/marky-markdown)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-marky-markdown/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-marky-markdown/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-marky-markdown/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-marky-markdown/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-marky-markdown/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-marky-markdown/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-marky-markdown/tree/gh-pages/build)|

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-marky-markdown/build/screenCapture.buildCustomOrg.browser.coverage.html.png)](https://npmtest.github.io/node-npmtest-marky-markdown/build/coverage.html/index.html)

[![test-report](https://npmtest.github.io/node-npmtest-marky-markdown/build/screenCapture.buildCustomOrg.browser.%252Fhome%252Ftravis%252Fbuild%252Fnpmtest%252Fnode-npmtest-marky-markdown%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-marky-markdown/build/test-report.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-marky-markdown/build/screenCapture.buildApidoc.browser.%252Fhome%252Ftravis%252Fbuild%252Fnpmdoc%252Fnode-npmdoc-marky-markdown%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-marky-markdown/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-marky-markdown/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-marky-markdown/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Ashley Williams",
        "email": "ashley@npmjs.com",
        "url": "http://ashleygwilliams.github.io/"
    },
    "bin": {
        "marky-markdown": "./bin/marky-markdown.js"
    },
    "browser": {
        "highlights": false
    },
    "bugs": {
        "url": "https://github.com/npm/marky-markdown/issues"
    },
    "dependencies": {
        "atom-language-diff": "^1.0.0",
        "atom-language-nginx": "^0.6.1",
        "github-slugger": "^1.0.0",
        "github-url-to-object": "^2.2.3",
        "highlights": "^2.1.3",
        "highlights-tokens": "^1.0.1",
        "innertext": "^1.0.1",
        "is-badge": "^1.1.0",
        "language-dart": "^0.1.1",
        "language-erlang": "^2.0.0",
        "language-glsl": "^2.0.1",
        "language-haxe": "^0.2.1",
        "language-ini": "^1.7.0",
        "language-rust": "^0.4.7",
        "language-stylus": "^0.5.2",
        "lodash.assign": "^4.0.2",
        "lodash.defaults": "^4.0.1",
        "lodash.pickby": "^4.2.1",
        "markdown-it": "^8.0.0",
        "markdown-it-emoji": "^1.3.0",
        "markdown-it-expand-tabs": "^1.0.7",
        "markdown-it-lazy-headers": "^0.1.3",
        "markdown-it-task-lists": "^1.0.0",
        "property-ttl": "^1.0.0",
        "sanitize-html": "^1.6.1",
        "similarity": "^1.0.1"
    },
    "description": "npm's markdown parser",
    "devDependencies": {
        "browserify": "^13.0.1",
        "cheerio": "^0.22.0",
        "glob": "^7.1.1",
        "intercept-stdout": "^0.1.2",
        "mocha": "^3.1.2",
        "standard": "^8.4.0",
        "standard-format": "^2.1.0"
    },
    "directories": {},
    "dist": {
        "shasum": "cd3f20812992a5d6b440abe160bfca0f760b3ed0",
        "tarball": "https://registry.npmjs.org/marky-markdown/-/marky-markdown-9.0.2.tgz"
    },
    "gitHead": "fce972776b677ec7a6cb0bdc2f3054b0d89d328b",
    "homepage": "https://github.com/npm/marky-markdown",
    "keywords": [
        "readme",
        "markdown",
        "md",
        "documentation",
        "syntax highlighting",
        "html",
        "github",
        "npm"
    ],
    "license": "ISC",
    "main": "index.js",
    "maintainers": [
        {
            "name": "ag_dubs",
            "email": "ashley666ashley@gmail.com"
        },
        {
            "name": "bcoe",
            "email": "ben@npmjs.com"
        },
        {
            "name": "revin",
            "email": "rg@sevenite.com"
        },
        {
            "name": "rockbot",
            "email": "raquel@rckbt.me"
        },
        {
            "name": "soldair",
            "email": "soldair@gmail.com"
        }
    ],
    "name": "marky-markdown",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/npm/marky-markdown.git"
    },
    "scripts": {
        "build": "rm -rf dist && mkdir dist && touch dist/marky-markdown.js && browserify index.js -i highlights -s markyMarkdown > dist/marky-markdown.js",
        "pretest": "npm run build",
        "test": "standard-format -w && standard && mocha --timeout 8000"
    },
    "standard": {
        "ignore": "dist"
    },
    "version": "9.0.2"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
