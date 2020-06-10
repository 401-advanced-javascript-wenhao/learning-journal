# Class 42 - SMACSS & React Native Recap - 6/9/2020

## SMACSS - Scalable and Modular Architecture for CSS

1. Base - base rules are the defaults.

```css
html,
body,
form {
  margin: 0;
  padding: 0;
}
input[type="text"] {
  border: 1px solid #999;
}
a {
  color: #039;
}
a:hover {
  color: #03c;
}
```

2. Layout - divide the page into sections. Layouts hold one or more modules together.
3. Module - resuable, modular parts of our design. They are the callouts, the sidebar section, the product lists and so on.
4. State - ways to describe how our modules or layouts will look when in a particular state. Is it hidden or expanded? Is it active or inactive? etc.
5. Theme - similar to state rules in that they describe how modules or layouts might look. Most sites don't require a layer of theming but it is good to be aware of it.

## React Native Ecosystem

- Native development - using native machine code to run apps connected directly to hardware and OS features
- Performance and quality are preserved
- Consistent user experience
- It's still just state and components
  - But no HTML or CSS
  - You can still "style" things using the framework guidelines

## Expo

- expo is the dev environment
- snack is online sandbox
- expo-cli is the local equivalent to create-react-app (you can eject)
- running locally, you can use your own device or the official simulator
  - only Apple users can test iphones
  - Anyone can test android, but you need to start up an ADB from the Android Studio IDE
