# DOOM: Bean

DOOM bridge for the Bean event framework.


### Example

```
// Require bean and instantiate DOOM using it for the eventing stuff
var bean = require('doom-bean')
var doom = require('doom')(undefined, bean)

// Then use DOOM event functions normally
doom.delegate('.clickable', 'click', doom.query('body'), function(ev, el) {
  ev.preventDefault()
  doom.addClass('active', el)
})
```


### Installing

Just grab it from NPM:

    $ npm install doom-bean


### Licence

MIT/X11. ie.: do whatever you want.

[Calliope]: https://github.com/killdream/calliope
[es5-shim]: https://github.com/kriskowal/es5-shim
