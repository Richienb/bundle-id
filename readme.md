# bundle-id [![Build Status](https://travis-ci.org/sindresorhus/bundle-id.svg?branch=master)](https://travis-ci.org/sindresorhus/bundle-id)

> Get [bundle identifier](https://developer.apple.com/library/Mac/documentation/General/Reference/InfoPlistKeyReference/Articles/CoreFoundationKeys.html#//apple_ref/doc/plist/info/CFBundleIdentifier) from a [bundle name](https://developer.apple.com/library/Mac/documentation/General/Reference/InfoPlistKeyReference/Articles/CoreFoundationKeys.html#//apple_ref/doc/plist/info/CFBundleName) (OS X): `Safari` => `com.apple.Safari`

See [bundle-name](https://github.com/sindresorhus/bundle-name) for the reverse.


## Install

```bash
$ npm install --save bundle-id
```


## Usage

```js
var bundleId = require('bundle-id');

bundleId('Safari', function (err, id) {
	console.log(id);
	//=> com.apple.Safari
});
```


## CLI

You can also use it as a CLI app by installing it globally:

```
npm install --global bundle-id
```

### Usage

```
bundle-id Safari
```

Which will output `com.apple.Safari`.


## License

[MIT](http://opensource.org/licenses/MIT) © [Sindre Sorhus](http://sindresorhus.com)
