# Class 4 - Advanced MongoDB/Mongoose - 4/16/2020

## Setup & Install dependencies
  * `npm install --save mongoose`
  * `npm install --save-dev jest mongodb-memory-server`


## Mongoose Schema and Model
```javascript
const mongoose = require('mongoose');

const food = mongoose.Schema({
  name: { type: String, required: true },
  calories: { type: Number, required: true },
  type: { type: String, required: true, uppercase: true, enum: ['FRUIT', 'VEG', 'MEAT']}
});

module.exports = mongoose.model('food', food);
```

## In Memory Database Testing
* Pros:
  * No mocks needed
  * Faster development cycle
  * Testing the code that will be in production, not an old/incorrect/incomplete mock
  * Esay to write the test
* Cons:
  * Needs to seed the database
  * Needs more memory
  * Tests take longer time to run