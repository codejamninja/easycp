# easycp

[![Beerpay](https://beerpay.io/jamrizzi/easycp/make-wish.svg?style=flat-square)](https://beerpay.io/jamrizzi/easycp?focus=wish)
[![GitHub stars](https://img.shields.io/github/stars/jamrizzi/easycp.svg?style=social&label=Stars)](https://github.com/jamrizzi/easycp)

> Easy child process

Please ★ this repo if you found it useful ★ ★ ★


# Features

* Promise based
* Works with i/o


# Installation

```sh
npm install --save easycp
```


# Dependencies

* [NodeJS](https://nodejs.org)


# Usage

```js
import easycp, { readcp, silentcp } from 'easycp';

// streams to stdout and process returned
easycp('echo hello world').then(process => console.log(process)); // [object Object]

// alternative syntax
easycp('echo', ['hello', 'world']).then(process => console.log(process)); // [object Object]

// streams to stdout (stderr silenced) and process returned
easycp('echo', ['hello', 'world'], { stderr: false }).then(process => console.log(process)); // [object Object]

// stream silenced and process returned
silentcp('echo hello world').then(process => console.log(process)); // [object Object]

// stream silenced and returned as result
readcp('echo hello world').then(result => console.log(result)); // hello world
```


# Support

Submit an [issue](https://github.com/jamrizzi/easycp/issues/new)


# Contributing

Review the [guidelines for contributing](https://github.com/jamrizzi/easycp/blob/master/CONTRIBUTING.md)


# License

[MIT License](https://github.com/jamrizzi/easycp/blob/master/LICENSE)

[Jam Risser](https://jam.jamrizzi.com) © 2018


# Changelog

Review the [changelog](https://github.com/jamrizzi/easycp/blob/master/CHANGELOG.md)


# Credits

* [Jam Risser](https://jam.jamrizzi.com) - Author


# Support on Beerpay

A ridiculous amount of coffee :coffee: :coffee: :coffee: was consumed in the process of building this project.

[Add some fuel](https://beerpay.io/jamrizzi/easycp) if you'd like to keep me going!

[![Beerpay](https://beerpay.io/jamrizzi/easycp/make-wish.svg?style=flat-square)](https://beerpay.io/jamrizzi/easycp?focus=wish)
