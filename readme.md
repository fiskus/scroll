# scroll
A function that animates an element’s scrollTop value.

[![Build status](https://travis-ci.org/michaelrhodes/scroll.png?branch=master)](https://travis-ci.org/michaelrhodes/scroll)

[![Browser support](https://ci.testling.com/michaelrhodes/scroll.png)](https://ci.testling.com/michaelrhodes/scroll)

## Install
```
npm install scroll
```

### API
```
  scroll(
    element (element),
    target (number): the desired scrollTop position,
    options (object): { duration, ease },
    callback (function): fn(error, position)
  ) 
```
Note: The easing functions are those specified in [component/ease](https://github.com/component/ease).

### Example
``` js
var scroll = require('scroll')

var element = document.body

scroll.top(element, 200, { duration: 1000 }, function(error, position) {})
scroll.left(element, 200, { ease: 'inBounce' }, function(error, position) {})
```

### License
[MIT](http://opensource.org/licenses/MIT)
