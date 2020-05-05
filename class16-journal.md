# Class 16 - Event Driven Applications - 5/4/2020

* Everything in JS is an object. Arrays, functions, documents, windows are all objects.
* Most action in JS are event driven.
  * UI Events - click, keyboard press down, scroll, hover, zoom etc
  * Express routes
  * Model Lifecycle Hooks
  * React Components - ES6 class
* Modern browser comes with a lot of handy events we can use such as click, scroll, hover, zoom etc.
* In JS, we can use events module in Node.js to create custom events and use emit method to fire registered events.
* Example: <br/>
```javascript
const EE = require('events');
const events = new EE();
events.on('pickup', function(payload) {/* do something */}); // register a function
events.emit('pickup', payload); // fire registered function
```
