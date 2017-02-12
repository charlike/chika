<h1 align="center">Chika 
  <a href="https://www.npmjs.com/package/mich-to-html"><img src="https://img.shields.io/npm/v/resolve-package.svg?style=flat" alt="npm version"></a>
  <a href="https://www.npmjs.com/package/mich-to-html"><img src="https://img.shields.io/npm/l/resolve-package.svg?style=flat" alt="npm version"></a>
  <a href="https://npmjs.org/package/mich-to-html"><img src="https://img.shields.io/npm/dm/resolve-package.svg?style=flat" alt="npm downloads monthly"></a>
  <a href="https://npmjs.org/package/mich-to-html"><img src="https://img.shields.io/npm/dt/resolve-package.svg?style=flat" alt="npm downloads total"></a>
  <br>
<img src="http://www.wallpaperscharlie.com/wp-content/uploads/2016/07/Cute-Girls-HD-Pictures-9.jpg" alt="Chika - Build brilliant UI apps, fast & easy." width="90%" height="90%"><br>
Build brilliant UI apps, fast & easy.
</h1>

> Chika is sweety little chick in the JavaScript _\_ecosphere_\_ that creates blazing fast &amp; gorgeous apps.

<!--<p align="center">
  <a href="https://codeclimate.com/github/tunnckoCore/mich-to-html"><img src="https://img.shields.io/codeclimate/github/tunnckoCore/resolve-package.svg" alt="codeclimate"></a>
  <a href="https://github.com/feross/standard"><img src="https://img.shields.io/badge/code%20style-standard-brightgreen.svg" alt="codestyle"></a>
  <a href="https://travis-ci.org/tunnckoCore/mich-to-html"><img src="https://img.shields.io/travis/tunnckoCore/resolve-package/master.svg?label=linux" alt="travis"></a>
  <a href="https://ci.appveyor.com/project/tunnckoCore/mich-to-html"><img src="https://img.shields.io/appveyor/ci/tunnckoCore/resolve-package/master.svg?label=windows" alt="appveyor"></a>
  <a href="https://codecov.io/gh/tunnckoCore/mich-to-html"><img src="https://img.shields.io/coveralls/tunnckoCore/resolve-package.svg" alt="codecov"></a>
  <a href="https://david-dm.org/tunnckoCore/mich-to-html"><img src="https://img.shields.io/david/tunnckoCore/resolve-package.svg" alt="david-dm"></a>
</p>-->

[![code climate][codeclimate-img]][codeclimate-url] 
[![standard code style][standard-img]][standard-url] 
[![linux build status][travis-img]][travis-url] 
[![windows build status][appveyor-img]][appveyor-url] 
[![coverage status][coveralls-img]][coveralls-url] 
[![dependency status][david-img]][david-url]

_You might also be interested in [mich-h][] - virtual dom builder in just ~500 bytes, compatible with [hyperscript][]._

## Table of Contents
- [Install](#install)
- [Usage](#usage)
- [Background](#background)
  * [What and Why?](#what-and-why)
  * [Resolution](#resolution)
- [API](#api)
  * [resolvePluginsSync](#resolvepluginssync)
- [Related](#related)
- [Contributing](#contributing)
- [Building docs](#building-docs)
- [Running tests](#running-tests)
- [Author](#author)
- [License](#license)

_(TOC generated by [verb](https://github.com/verbose/verb) using [markdown-toc](https://github.com/jonschlinkert/markdown-toc))_

## Install
Install with [npm](https://www.npmjs.com/)

```
$ npm install resolve-plugins-sync --save
```

or install using [yarn](https://yarnpkg.com)

```
$ yarn add resolve-plugins-sync
```

## Usage
> For more use-cases see the [tests](test.js)

```js
const resolvePluginsSync = require('resolve-plugins-sync')

// fake
const baz = require('tool-plugin-baz')
const qux = require('tool-plugin-qux')

const result = resolvePluginsSync([
  'foo',
  ['bar', { some: 'options here' }],
  [baz, { a: 'b' }],
  qux
], {
  prefix: 'tool-plugin-'
})
```

## Contributing
Pull requests and stars are always welcome. For bugs and feature requests, [please create an issue](https://github.com/tunnckoCore/resolve-plugins-sync/issues/new).  
Please read the [contributing guidelines](CONTRIBUTING.md) for advice on opening issues, pull requests, and coding standards.  
If you need some help and can spent some cash, feel free to [contact me at CodeMentor.io](https://www.codementor.io/tunnckocore?utm_source=github&utm_medium=button&utm_term=tunnckocore&utm_campaign=github) too.

**In short:** If you want to contribute to that project, please follow these things

1. Please DO NOT edit [README.md](README.md), [CHANGELOG.md](CHANGELOG.md) and [.verb.md](.verb.md) files. See ["Building docs"](#building-docs) section.
2. Ensure anything is okey by installing the dependencies and run the tests. See ["Running tests"](#running-tests) section.
3. Always use `npm run commit` to commit changes instead of `git commit`, because it is interactive and user-friendly. It uses [commitizen][] behind the scenes, which follows Conventional Changelog idealogy.
4. Do NOT bump the version in package.json. For that we use `npm run release`, which is [standard-version][] and follows Conventional Changelog idealogy.

Thanks a lot! :)

## Building docs
Documentation and that readme is generated using [verb-generate-readme][], which is a [verb][] generator, so you need to install both of them and then run `verb` command like that

```
$ npm install verbose/verb#dev verb-generate-readme --global && verb
```

_Please don't edit the README directly. Any changes to the readme must be made in [.verb.md](.verb.md)._

## Running tests
Clone repository and run the following in that cloned directory

```
$ npm install && npm test
```

## Author
**Charlike Mike Reagent**

+ [github/tunnckoCore](https://github.com/tunnckoCore)
+ [twitter/tunnckoCore](https://twitter.com/tunnckoCore)
+ [codementor/tunnckoCore](https://codementor.io/tunnckoCore)

## License
Copyright © 2016-2017, [Charlike Mike Reagent](https://i.am.charlike.online). Released under the [MIT license](LICENSE).

***

_This file was generated by [verb-generate-readme](https://github.com/verbose/verb-generate-readme), v0.4.2, on February 12, 2017._  
_Project scaffolded using [charlike][] cli._



[always-done]: https://github.com/hybridables/always-done
[async-done]: https://github.com/gulpjs/async-done
[base]: https://github.com/node-base/base
[charlike]: https://github.com/tunnckocore/charlike
[commitizen]: https://github.com/commitizen/cz-cli
[detect-installed]: https://github.com/tunnckocore/detect-installed
[dezalgo]: https://github.com/npm/dezalgo
[generate]: https://github.com/generate/generate
[get-installed-path]: https://github.com/tunnckocore/get-installed-path
[global-modules]: https://github.com/jonschlinkert/global-modules
[global-prefix]: https://github.com/jonschlinkert/global-prefix
[gulp]: http://gulpjs.com
[is-installed]: https://github.com/tunnckoCore/is-installed
[once]: https://github.com/isaacs/once
[resolve-from]: https://github.com/sindresorhus/resolve-from
[resolve-module]: https://github.com/jkroso/node-resolve-module
[resolve-pkg]: https://github.com/sindresorhus/resolve-pkg
[resolve]: https://github.com/substack/node-resolve
[standard-version]: https://github.com/conventional-changelog/standard-version
[verb-generate-readme]: https://github.com/verbose/verb-generate-readme
[verb]: https://github.com/verbose/verb

[downloads-url]: https://www.npmjs.com/package/resolve-package
[downloads-img]: https://img.shields.io/npm/dt/resolve-package.svg

[codeclimate-url]: https://codeclimate.com/github/tunnckoCore/resolve-package
[codeclimate-img]: https://img.shields.io/codeclimate/github/tunnckoCore/resolve-package.svg

[travis-url]: https://travis-ci.org/tunnckoCore/resolve-package
[travis-img]: https://img.shields.io/travis/tunnckoCore/resolve-package/master.svg?label=linux

[appveyor-url]: https://ci.appveyor.com/project/tunnckoCore/resolve-package
[appveyor-img]: https://img.shields.io/appveyor/ci/tunnckoCore/resolve-package/master.svg?label=windows

[coveralls-url]: https://coveralls.io/r/tunnckoCore/resolve-package
[coveralls-img]: https://img.shields.io/coveralls/tunnckoCore/resolve-package.svg

[david-url]: https://david-dm.org/tunnckoCore/resolve-package
[david-img]: https://img.shields.io/david/tunnckoCore/resolve-package.svg

[standard-url]: https://github.com/feross/standard
[standard-img]: https://img.shields.io/badge/code%20style-standard-brightgreen.svg
