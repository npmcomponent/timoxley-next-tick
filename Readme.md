*This repository is a mirror of the [component](http://component.io) module [timoxley/next-tick](http://github.com/timoxley/next-tick). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/timoxley-next-tick`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*

# next-tick

  process.nextTick for browser.

## Installation

    $ component install timoxley/next-tick

## Example

```js

// This example sucks.

var nextTick = require('next-tick')

var i = 0;

nextTick(function() {
	i++ // i === 2
})

i++ // i === 1
```

## Further reading 

This implementation mirrors the behaviour of node's `process.nextTick`. Therefore, it comes with all the same benefits and caveats. see node's [documentation](http://nodejs.org/api/process.html#process_process_nexttick_callback) for details 

## Credit

Adapted from [mocha codebase](https://github.com/visionmedia/mocha/blob/142c69991a2f39c0add38ba1d202c094e69d81f9/support/tail.js#L19).

## License

  MIT
