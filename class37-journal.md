# Class 37 - Redux: Combined Reducers - 6/2/2020  

## Combined Reducers  
* Pulling in more than one reducers from source and creating a keyed object from them 
* Any component can reach into the store and use state  
* Obey Single Source of Truth 
* Each reducer technically has its own actions and creators 
* However, they can cross over and both be dispatched 
  * Example:
  ```javascript
  // counter-store.js -> reducer1
  export default function reducer1 (state = initialState, action) {
    const { type, payload } = action;
    switch(type) {
      case 'INCREMENT':
        return { value: state.value + 1};
      
      case 'RESET':
        return { value: 0 };

      default:
        return state;
    }
  }


  // history-store.js -> reducer2
  export default function reducer2 (state = initialState, action) {
    const { type, payload } = action;
    switch(type) {
      case 'CLICK':
        return { clicks: state.clicks + 1 };

      case 'RESET':
        return { clicks: 0 };

      default:
        return state;
    }
  }

  // combine two reducers in /src/store/index.js
  import { createStore, combineReducers } from 'redux';
  import reducer1 from './counter-store.js';
  import reducer2 from './history-store.js';
  const reducers = combineReducers({ reducer1, reducer2 });
  ```