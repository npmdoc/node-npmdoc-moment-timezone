# npmdoc-moment-timezone

#### api documentation for  [moment-timezone (v0.5.13)](http://momentjs.com/timezone/)  [![npm package](https://img.shields.io/npm/v/npmdoc-moment-timezone.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-moment-timezone) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-moment-timezone.svg)](https://travis-ci.org/npmdoc/node-npmdoc-moment-timezone)

#### Parse and display moments in any timezone.

[![NPM](https://nodei.co/npm/moment-timezone.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/moment-timezone)

- [https://npmdoc.github.io/node-npmdoc-moment-timezone/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-moment-timezone/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-moment-timezone/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-moment-timezone/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-moment-timezone/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-moment-timezone/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "moment-timezone",
    "version": "0.5.13",
    "description": "Parse and display moments in any timezone.",
    "homepage": "http://momentjs.com/timezone/",
    "author": "Tim Wood <washwithcare@gmail.com> (http://timwoodcreates.com/)",
    "keywords": [
        "moment",
        "date",
        "time",
        "timezone",
        "olson",
        "iana",
        "zone",
        "tz"
    ],
    "main": "./index.js",
    "engines": {
        "node": "*"
    },
    "repository": {
        "type": "git",
        "url": "https://github.com/moment/moment-timezone.git"
    },
    "bugs": {
        "url": "https://github.com/moment/moment-timezone/issues"
    },
    "license": "MIT",
    "dependencies": {
        "moment": ">= 2.9.0"
    },
    "devDependencies": {
        "grunt": "0.4.5",
        "grunt-contrib-clean": "0.6.0",
        "grunt-contrib-nodeunit": "0.4.1",
        "grunt-contrib-jshint": "0.11.2",
        "grunt-contrib-uglify": "0.9.1"
    },
    "jspm": {
        "main": "builds/moment-timezone-with-data",
        "shim": {
            "moment-timezone": {
                "deps": [
                    "moment"
                ]
            }
        }
    },
    "scripts": {
        "test": "grunt"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
