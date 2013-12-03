enter
=====

Event trigger router, like hash route;


## sample

```javascript
var enterId = enter('click .onlog', global.onlog, view.render);

enter('change .input', global.input, view.renderInp);
// delegate
enter('body:click .button', global.onlog, view.renderButton);
// hash route
enter('route', global.onlog, view.renderButton);
// rebinding event
enter.reflesh('click .onlog');
// like enter('click .onlog', global.onlog, view.render)
enter.bind('click .onlog', global.onlog, view.render);
// unbind with id
enter.unbind('click .onlog', enterId);
// tigger event
enter.trigger('click .onlog', target, [options])
// unbind all
enter.reset();

```
