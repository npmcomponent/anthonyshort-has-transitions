*This repository is a mirror of the [component](http://component.io) module [anthonyshort/has-transitions](http://github.com/anthonyshort/has-transitions). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/anthonyshort-has-transitions`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*

# has-transitions

  Determine if an element has transitions

## Installation

    $ component install anthonyshort/has-transitions

or via npm for Browserify

    $ npm install has-transitions

## API

    var hasTransitions = require('has-transitions');
    var cssEmitter = require('css-emitter');

    if(hasTransitions(el)) {
      cssEmitter(el).bind(onTransitionEnd);
    }
    else {
      onTransitionEnd();
    }

## Methods

### hasTransitions([el])

Determine if an element has any transition properties. If the browser doesn't
support transitions this will always return false.

If `el` isn't passed it will return a boolean for browser support for transitions.

## License

  MIT
