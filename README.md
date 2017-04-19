# npmdoc-gauge

#### api documentation for  [gauge (v2.7.3)](https://github.com/iarna/gauge)  [![npm package](https://img.shields.io/npm/v/npmdoc-gauge.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-gauge) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-gauge.svg)](https://travis-ci.org/npmdoc/node-npmdoc-gauge)

#### A terminal based horizontal guage

[![NPM](https://nodei.co/npm/gauge.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/gauge)

- [https://npmdoc.github.io/node-npmdoc-gauge/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-gauge/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-gauge/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-gauge/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-gauge/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-gauge/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Rebecca Turner"
    },
    "bugs": {
        "url": "https://github.com/iarna/gauge/issues"
    },
    "dependencies": {
        "aproba": "^1.0.3",
        "console-control-strings": "^1.0.0",
        "has-unicode": "^2.0.0",
        "object-assign": "^4.1.0",
        "signal-exit": "^3.0.0",
        "string-width": "^1.0.1",
        "strip-ansi": "^3.0.1",
        "wide-align": "^1.1.0"
    },
    "description": "A terminal based horizontal guage",
    "devDependencies": {
        "readable-stream": "^2.0.6",
        "require-inject": "^1.4.0",
        "standard": "^7.1.2",
        "tap": "^5.7.2",
        "through2": "^2.0.0"
    },
    "directories": {},
    "dist": {
        "shasum": "1c23855f962f17b3ad3d0dc7443f304542edfe09",
        "tarball": "https://registry.npmjs.org/gauge/-/gauge-2.7.3.tgz"
    },
    "files": [
        "base-theme.js",
        "CHANGELOG.md",
        "error.js",
        "has-color.js",
        "index.js",
        "LICENSE",
        "package.json",
        "plumbing.js",
        "process.js",
        "progress-bar.js",
        "README.md",
        "render-template.js",
        "set-immediate.js",
        "set-interval.js",
        "spin.js",
        "template-item.js",
        "theme-set.js",
        "themes.js",
        "wide-truncate.js"
    ],
    "gitHead": "2defcdb50c243c92d21f0fd39c4b06bd48bcfdf3",
    "homepage": "https://github.com/iarna/gauge",
    "keywords": [
        "progressbar",
        "progress",
        "gauge"
    ],
    "license": "ISC",
    "main": "index.js",
    "maintainers": [
        {
            "name": "iarna"
        }
    ],
    "name": "gauge",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/iarna/gauge.git"
    },
    "scripts": {
        "prepublish": "rm -f *~",
        "test": "standard && tap test/*.js --coverage"
    },
    "version": "2.7.3"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
