# camelcase-keys [![Build Status](https://travis-ci.org/sindresorhus/camelcase-keys.svg?branch=master)](https://travis-ci.org/sindresorhus/camelcase-keys)

> Convert object keys to camelCase using [`camelcase`](https://github.com/sindresorhus/camelcase)


## Install

```
$ npm install --save camelcase-keys
```


## Usage

```js
const camelcaseKeys = require('camelcase-keys');

camelcaseKeys({'foo-bar': true});
//=> {fooBar: true}


const argv = require('minimist')(process.argv.slice(2));
//=> {_: [], 'foo-bar': true}

camelcaseKeys(argv);
//=> {_: [], fooBar: true}
```


## API

### camelcaseKeys(obj, [exclude])

#### obj

Type: `Object`

Object to camelCase.

#### exclude

Type: `Array`  
Default: `[]`

Exclude keys from camelCasing.


## License

MIT © [Sindre Sorhus](http://sindresorhus.com)
