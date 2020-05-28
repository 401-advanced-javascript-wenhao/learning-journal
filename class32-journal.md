# Class 32 - Custom Hooks - 5/27/2020 

## State Hook VS Custom Hook  
I learned state hook yesterday. It enables function component to maintain its own state and it makes code neat and dry. But one thing I figured out was if there are several input fileds, I have to make seperate similar function for handle change for each input field. There was a lot of repetitive codes. I learned custom hook today and it perfectly solved this problem.  

## Custom Hooks 
* Extract duplicated logic from components
* Share common functionality not state
* Take advantage of useEffect lifecycle
* Common use cases - make coding neat and dry
  * Handle Forms
  * Pre-fetch API data
  * Connect to services (socket.io, Q, etc) 

## How does custom hooks work 
* Hooks are exported as a function, named as useXXX()
* Hooks return data or functions that are required to reuse their internal functionality
* Hooks are imported into components
* Components can re-use the hook functionality or data/state as needed
* Hooks do not render Example:  
```javascript
// create custom hooks in the use-food-hook.js and export it
export default function useFoodHook(hungry) {
  const foot = 'cookies';
  return hungry ? food : null;
}

// import custom hooks and use it
import useFeedme from 'use-food-hook.js';
const myComponent = props => {
  const food = useFeedMe(true);
  return <div>{food}</div>
}
```