# Class 36 - Application state with Redux - 6/1/2020  
Redux is a library that specializes in sharing state between components using a global "store".

## How does redux work  
* Action: an object with a type and payload 
* Action creators: pure functions that return an action 
* Reducers: evaluate the `type` property on an action and makes a copy of the state, given the payload  
* Reducers get included into the creation of store - the single object of tree holding in the app with `createStore(reducer)` 
* Application access this state through use of a `react-redux` npm module that gives us a `<Provider>` component  
* `<Provider>` component has a prop called `store` that takes in the state and feeds it to our entire app 
* `mapDispatchToProps`: assigns action creators to props  
* `mapStateToProps`: assigns state properties to component level props  

## Redux Store  
* Where application state is stored
* Identify various reducers and middleware that need to be made available and used globally
* React uses `reducers` to hold and manage state
* Reducer manage just one part of the larger application state
* Reducer creates an initial "empty" state and then evaluates action and make a copy of state accordingly
* Reducers hear the `dispatch` and `payload`