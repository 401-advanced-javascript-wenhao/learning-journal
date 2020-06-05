# Class 39 - Redux Toolkit - 6/4/2020 
Redux is great, but there is a lot of "boilerplate" code that we have to write, and every developer or company will have their own internal pattern for putting it all together.
  * File and Directory Names  
  * Reducer and Action Styles 
  * How do we model our data in the reducers  

## Redux Toolkit  
* Introduced by Redux developer team  
* Specifies a few different means of building a reducer and action set that work well together and are easier to understand and integrate 
* Example:  
```javascript
const postsSlice = createSlice({
  name: 'posts',
  initialState: [],
  reducers: {
    createPost(state, action) {},
    updatePost(state, action) {},
    deletePost(state, action) {}
  }
})

// Extract the action creators object and the reducer 
const { actions, reducer } = postsSlice;
// Extract and export each action creator by name
export const { createPost, updatePost, deletePost } = actions;
// Export the reducer, either as a default or named export
export default reducer;

// ----- Sample Use -----
console.log(createPost({ id:123, title: 'Hello World }));

{type: "posts/createPost", payload: {id: 123, title: "Hello World"}}

// Notice how createSlice transforms your definition.
console.log(postSlice);
{ name: 'posts', actions: { createPost, updatePost, deletePost }, reducer}
```