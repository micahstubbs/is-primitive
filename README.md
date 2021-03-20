# is-primitive [![NPM version](https://img.shields.io/npm/v/is-primitive.svg?style=flat)](https://www.npmjs.com/package/is-primitive) [![NPM monthly downloads](https://img.shields.io/npm/dm/is-primitive.svg?style=flat)](https://npmjs.org/package/is-primitive) [![NPM total downloads](https://img.shields.io/npm/dt/is-primitive.svg?style=flat)](https://npmjs.org/package/is-primitive) [![Linux Build Status](https://img.shields.io/travis/jonschlinkert/is-primitive.svg?style=flat&label=Travis)](https://travis-ci.org/jonschlinkert/is-primitive)

> Returns `true` if the value is a primitive.

Please consider following this project's author, [Jon Schlinkert](https://github.com/jonschlinkert), and consider starring the project to show your :heart: and support.

## Install

Install with [npm](https://www.npmjs.com/):

```sh
$ npm install --save is-primitive
```

## Primitive values

The [Mozilla docs for "Primitive values"](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures#Primitive_values) defines specifies seven data types that are primitives:

* `Boolean`
* `Null`
* `Undefined`
* `Number`
* `String`
* `Symbol` (new in ECMAScript 6)
* `BigInt` (new in ECMAScript 2020)

## Usage

```js
var isPrimitive = require('is-primitive');
```

## true

All of the following return `true`:

```js
console.log(isPrimitive(false));
console.log(isPrimitive(true));
console.log(isPrimitive(null));
console.log(isPrimitive());
console.log(isPrimitive(42));
console.log(isPrimitive('abc'));
console.log(isPrimitive(Symbol()));
//=> true
```

## false

Everything else returns `false`:

```js
console.log(isPrimitive({}));
console.log(isPrimitive([]));
console.log(isPrimitive(function(){}));
console.log(isPrimitive(new Date()));
// et cetera...
//=> false
```

## About

<details>
<summary><strong>Contributing</strong></summary>

Pull requests and stars are always welcome. For bugs and feature requests, [please create an issue](../../issues/new).

</details>

<details>
<summary><strong>Running Tests</strong></summary>

Running and reviewing unit tests is a great way to get familiarized with a library and its API. You can install dependencies and run tests with the following command:

```sh
$ npm install && npm test
```

</details>

<details>
<summary><strong>Building docs</strong></summary>

_(This project's readme.md is generated by [verb](https://github.com/verbose/verb-generate-readme), please don't edit the readme directly. Any changes to the readme must be made in the [.verb.md](.verb.md) readme template.)_

To generate the readme, run the following command:

```sh
$ npm install -g verbose/verb#dev verb-generate-readme && verb
```

</details>

### Related projects

You might also be interested in these projects:

* [is-number](https://www.npmjs.com/package/is-number): Returns true if the value is a number. comprehensive tests. | [homepage](https://github.com/jonschlinkert/is-number "Returns true if the value is a number. comprehensive tests.")
* [is-plain-object](https://www.npmjs.com/package/is-plain-object): Returns true if an object was created by the `Object` constructor. | [homepage](https://github.com/jonschlinkert/is-plain-object "Returns true if an object was created by the `Object` constructor.")
* [kind-of](https://www.npmjs.com/package/kind-of): Get the native type of a value. | [homepage](https://github.com/jonschlinkert/kind-of "Get the native type of a value.")

### Contributors

| **Commits** | **Contributor** | 
| --- | --- |
| 11 | [jonschlinkert](https://github.com/jonschlinkert) |
| 1 | [ljharb](https://github.com/ljharb) |
| 1 | [bttmly](https://github.com/bttmly) |
| 1 | [hemanth](https://github.com/hemanth) |

### Author

**Jon Schlinkert**

* [github/jonschlinkert](https://github.com/jonschlinkert)
* [twitter/jonschlinkert](https://twitter.com/jonschlinkert)

### License

Copyright © 2017, [Jon Schlinkert](https://github.com/jonschlinkert).
Released under the [MIT License](LICENSE).

***

_This file was generated by [verb-generate-readme](https://github.com/verbose/verb-generate-readme), v0.6.0, on November 23, 2017._
