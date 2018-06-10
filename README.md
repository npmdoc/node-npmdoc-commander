# npmdoc-commander

#### basic api documentation for  [commander (2.15.1)](https://github.com/tj/commander.js#readme)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-commander.svg)](https://travis-ci.org/npmdoc/node-npmdoc-commander)

#### the complete solution for node.js command-line programs

[![NPM](https://nodei.co/npm/commander.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/commander)

- [https://npmdoc.github.io/node-npmdoc-commander/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-commander/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-commander/build/screenshot.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-commander/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-commander/build/screenshot.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-commander/build/screenshot.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "TJ Holowaychuk"
    },
    "bugs": {
        "url": "https://github.com/tj/commander.js/issues"
    },
    "dependencies": {},
    "description": "the complete solution for node.js command-line programs",
    "devDependencies": {
        "@types/node": "^7.0.55",
        "eslint": "^3.19.0",
        "should": "^11.2.1",
        "sinon": "^2.4.1",
        "standard": "^10.0.3",
        "typescript": "^2.7.2"
    },
    "directories": {},
    "dist": {
        "integrity": "sha512-VlfT9F3V0v+jr4yxPc5gg9s62/fIVWsd2Bk2iD435um1NlGMYdVCq+MjcXnhYq2icNOizHr1kK+5TI6H0Hy0ag==",
        "shasum": "df46e867d0fc2aec66a34662b406a9ccafff5b0f",
        "tarball": "https://registry.npmjs.org/commander/-/commander-2.15.1.tgz",
        "fileCount": 6,
        "unpackedSize": 59781
    },
    "files": [
        "index.js",
        "typings/index.d.ts"
    ],
    "gitHead": "649eaef336ddc7224eb5c73e4a958685e24de25e",
    "homepage": "https://github.com/tj/commander.js#readme",
    "keywords": [
        "commander",
        "command",
        "option",
        "parser"
    ],
    "license": "MIT",
    "main": "index",
    "maintainers": [
        {
            "name": "abetomo"
        },
        {
            "name": "somekittens"
        },
        {
            "name": "tjholowaychuk"
        },
        {
            "name": "vanesyan"
        },
        {
            "name": "zhiyelee"
        }
    ],
    "name": "commander",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/tj/commander.js.git"
    },
    "scripts": {
        "lint": "eslint index.js",
        "test": "make test && npm run test-typings",
        "test-typings": "node_modules/typescript/bin/tsc -p tsconfig.json"
    },
    "typings": "typings/index.d.ts",
    "version": "2.15.1",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
