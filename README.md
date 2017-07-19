# Karma tape adapter
> This Karma adapter reads [TAP](http://testanything.org/) output from runners like
[tape](https://github.com/substack/tape) into [Karma](http://karma-runner.github.io/1.0/index.html)

## Installation

### npm
```bash
npm install karma-tape-parser --save-dev
```
This was cloned from karma-tap. I just updated to the newest version of tap-parser because of several issues that was showing
up while running tests. It will follow the same structure as Karma tap.
https://github.com/bySabi/karma-tap/

## Configuration Example
`karma.conf.js`

```js
module.exports = function(config) {
  config.set({
    frameworks: ['browserify', 'tap'],
    files: [
      'test/**/*.js'
    ],
    preprocessors: {
      'test/**/*.js': [ 'browserify' ]
    }
  });
};
```

## TAP Protocol
Support TAP Protocol version `13`

## Credits

## License

[ISC][isc-license]

[isc-license]:./LICENSE
