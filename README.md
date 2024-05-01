# @devtea2028/fugit-facere-voluptates-ipsum <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

Get the ArrayBuffer out of a DataView, robustly.

This will work in node <= 0.10 and < 0.11.4, where there's no prototype accessor, only a nonconfigurable own property.
It will also work in modern engines where `DataView.prototype.buffer` has been deleted after this module has loaded.

## Example

```js
const dataViewBuffer = require('@devtea2028/fugit-facere-voluptates-ipsum');
const assert = require('assert');

const ab = new ArrayBuffer(0);
const dv = new DataView(ab);
assert.equal(dataViewBuffer(dv), ab);
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

[package-url]: https://npmjs.org/package/@devtea2028/fugit-facere-voluptates-ipsum
[npm-version-svg]: https://versionbadg.es/inspect-js/@devtea2028/fugit-facere-voluptates-ipsum.svg
[deps-svg]: https://david-dm.org/inspect-js/@devtea2028/fugit-facere-voluptates-ipsum.svg
[deps-url]: https://david-dm.org/inspect-js/@devtea2028/fugit-facere-voluptates-ipsum
[dev-deps-svg]: https://david-dm.org/inspect-js/@devtea2028/fugit-facere-voluptates-ipsum/dev-status.svg
[dev-deps-url]: https://david-dm.org/inspect-js/@devtea2028/fugit-facere-voluptates-ipsum#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@devtea2028/fugit-facere-voluptates-ipsum.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@devtea2028/fugit-facere-voluptates-ipsum.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@devtea2028/fugit-facere-voluptates-ipsum.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@devtea2028/fugit-facere-voluptates-ipsum
[codecov-image]: https://codecov.io/gh/inspect-js/@devtea2028/fugit-facere-voluptates-ipsum/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/inspect-js/@devtea2028/fugit-facere-voluptates-ipsum/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/inspect-js/@devtea2028/fugit-facere-voluptates-ipsum
[actions-url]: https://github.com/inspect-js/@devtea2028/fugit-facere-voluptates-ipsum/actions
