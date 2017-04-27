# npmtest-react-share

#### basic test coverage for  [react-share (v1.13.2)](https://github.com/nygardk/react-share#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-react-share.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-react-share) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-react-share.svg)](https://travis-ci.org/npmtest/node-npmtest-react-share)

#### Easy social media share buttons and share counts.

[![NPM](https://nodei.co/npm/react-share.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/react-share)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-react-share/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-react-share/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-react-share/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-react-share/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-react-share/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-react-share/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-react-share/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-react-share/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-react-share/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-react-share/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-react-share/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-react-share/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-react-share/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-react-share/build/test-report.html](https://npmtest.github.io/node-npmtest-react-share/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-react-share/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-react-share/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-react-share/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-react-share/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-react-share/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-react-share/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-react-share/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-react-share/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Klaus Nygård",
        "url": "http://klausnygard.fi"
    },
    "bugs": {
        "url": "https://github.com/nygardk/react-share/issues"
    },
    "dependencies": {
        "babel-runtime": "6.6.1",
        "classnames": "2.2.5",
        "jsonp": "0.2.1",
        "platform": "1.3.4",
        "prop-types": "^15.5.8"
    },
    "description": "Easy social media share buttons and share counts.",
    "devDependencies": {
        "babel-cli": "6.18.0",
        "babel-core": "6.18.2",
        "babel-eslint": "7.1.1",
        "babel-loader": "6.2.10",
        "babel-plugin-transform-class-properties": "6.18.0",
        "babel-plugin-transform-runtime": "6.15.0",
        "babel-preset-airbnb": "1.1.1",
        "babel-preset-es2015": "6.18.0",
        "babel-preset-react": "6.16.0",
        "babel-preset-stage-0": "6.16.0",
        "eslint": "2.13.1",
        "eslint-config-airbnb": "7.0.0",
        "eslint-loader": "1.6.3",
        "eslint-plugin-jsx-a11y": "0.6.2",
        "eslint-plugin-react": "4.3.0",
        "file-loader": "0.9.0",
        "react": "15.5.4",
        "react-dom": "15.5.4",
        "react-hot-loader": "1.3.1",
        "url-loader": "0.5.8",
        "webpack": "1.13.3",
        "webpack-dev-server": "1.16.3"
    },
    "directories": {},
    "dist": {
        "shasum": "21a5a6d419fd7ceb5a60dcd810cedb60e5a74185",
        "tarball": "https://registry.npmjs.org/react-share/-/react-share-1.13.2.tgz"
    },
    "engines": {
        "node": ">=4.0.0",
        "npm": ">=3.0.0"
    },
    "gitHead": "6a046f13cd8310373fda7c957e4f390cc10bbd25",
    "homepage": "https://github.com/nygardk/react-share#readme",
    "keywords": [
        "react",
        "component",
        "react-component",
        "social",
        "media",
        "social-media",
        "share",
        "button",
        "count"
    ],
    "license": "MIT",
    "main": "./lib/react-share.js",
    "maintainers": [
        {
            "name": "nyde"
        }
    ],
    "name": "react-share",
    "optionalDependencies": {},
    "peerDependencies": {
        "react": "0.13.x || 0.14.x || 15.x.x"
    },
    "repository": {
        "type": "git",
        "url": "git+https://github.com/nygardk/react-share.git"
    },
    "scripts": {
        "build": "npm run lint && npm run build-src && npm run build-demos",
        "build-demos": "NODE_ENV=production webpack -p --config webpack.demos.config.js",
        "build-src": "babel ./src --out-dir ./lib",
        "lint": "eslint --ext .jsx ./src ./demos",
        "prepublish": "npm run build",
        "run-demos": "NODE_ENV=development webpack-dev-server --config webpack.demos.config.js --content-base demos/ --progress --colors",
        "start": "npm run run-demos"
    },
    "version": "1.13.2",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
