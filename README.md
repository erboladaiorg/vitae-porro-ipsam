# @erboladaiorg/vitae-porro-ipsam <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

`Object.defineProperty`, but not IE 8's broken one.

## Example

```js
const assert = require('assert');

const $defineProperty = require('@erboladaiorg/vitae-porro-ipsam');

if ($defineProperty) {
    assert.equal($defineProperty, Object.defineProperty);
} else if (Object.defineProperty) {
    assert.equal($defineProperty, false, 'this is IE 8');
} else {
    assert.equal($defineProperty, false, 'this is an ES3 engine');
}
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

## Security

Please email [@ljharb](https://github.com/ljharb) or see https://tidelift.com/security if you have a potential security vulnerability to report.

[package-url]: https://npmjs.org/package/@erboladaiorg/vitae-porro-ipsam
[npm-version-svg]: https://versionbadg.es/ljharb/@erboladaiorg/vitae-porro-ipsam.svg
[deps-svg]: https://david-dm.org/ljharb/@erboladaiorg/vitae-porro-ipsam.svg
[deps-url]: https://david-dm.org/ljharb/@erboladaiorg/vitae-porro-ipsam
[dev-deps-svg]: https://david-dm.org/ljharb/@erboladaiorg/vitae-porro-ipsam/dev-status.svg
[dev-deps-url]: https://david-dm.org/ljharb/@erboladaiorg/vitae-porro-ipsam#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@erboladaiorg/vitae-porro-ipsam.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@erboladaiorg/vitae-porro-ipsam.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@erboladaiorg/vitae-porro-ipsam.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@erboladaiorg/vitae-porro-ipsam
[codecov-image]: https://codecov.io/gh/ljharb/@erboladaiorg/vitae-porro-ipsam/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/ljharb/@erboladaiorg/vitae-porro-ipsam/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/ljharb/@erboladaiorg/vitae-porro-ipsam
[actions-url]: https://github.com/erboladaiorg/vitae-porro-ipsam/actions
