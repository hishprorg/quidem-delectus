# @hishprorg/quidem-delectus <sup>[![Version Badge][2]][1]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![dependency status][5]][6]
[![dev dependency status][7]][8]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][11]][1]

Gets the description of a Symbol. Handles `Symbol()` vs `Symbol('')` properly when possible.

## Example

```js
var getSymbolDescription = require('@hishprorg/quidem-delectus');
var assert = require('assert');

assert(getSymbolDescription(Symbol()) === undefined);
assert(getSymbolDescription(Symbol('')) === ''); // or `undefined`, if in an engine that lacks name inference from concise method
assert(getSymbolDescription(Symbol('foo')) === 'foo');
assert(getSymbolDescription(Symbol.iterator) === 'Symbol.iterator');
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

[1]: https://npmjs.org/package/@hishprorg/quidem-delectus
[2]: https://versionbadg.es/inspect-js/@hishprorg/quidem-delectus.svg
[5]: https://david-dm.org/inspect-js/@hishprorg/quidem-delectus.svg
[6]: https://david-dm.org/inspect-js/@hishprorg/quidem-delectus
[7]: https://david-dm.org/inspect-js/@hishprorg/quidem-delectus/dev-status.svg
[8]: https://david-dm.org/inspect-js/@hishprorg/quidem-delectus#info=devDependencies
[11]: https://nodei.co/npm/@hishprorg/quidem-delectus.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@hishprorg/quidem-delectus.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@hishprorg/quidem-delectus.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@hishprorg/quidem-delectus
[codecov-image]: https://codecov.io/gh/inspect-js/@hishprorg/quidem-delectus/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/inspect-js/@hishprorg/quidem-delectus/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/inspect-js/@hishprorg/quidem-delectus
[actions-url]: https://github.com/hishprorg/quidem-delectus/actions
