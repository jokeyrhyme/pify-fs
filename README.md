# pify-fs [![npm](https://img.shields.io/npm/v/pify-fs.svg?maxAge=2592000)](https://www.npmjs.com/package/pify-fs) [![AppVeyor Status](https://ci.appveyor.com/api/projects/status/github/jokeyrhyme/pify-fs?branch=master&svg=true)](https://ci.appveyor.com/project/jokeyrhyme/pify-fs) [![Travis CI Status](https://travis-ci.org/jokeyrhyme/pify-fs.svg?branch=master)](https://travis-ci.org/jokeyrhyme/pify-fs)

Node.js' "fs" module, safer via graceful-fs, and more convenient via pify


## What is this?

I frequently use the awesome [graceful-fs](https://www.npmjs.com/package/graceful-fs) wrapper in combination with the convenient [pify](https://www.npmjs.com/package/pify) wrapper.

I got tired of doing this over and over again, so I made this module.


## Usage

```js
const fs = require('@jokeyrhyme/pify-fs')

fs.readdir(process.cwd())
  .then((files) => assert(Array.isArray(files)))
```

