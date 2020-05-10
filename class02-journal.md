# Class 2 - ES6 classes, Inheritance, Functional Programming - 4/14/2020

## Steps to build a Node.js package from scratch
1. Run command `npm init -y` from repo root directory to setup meta data for the package.
2. Run command `npm install package-name` to install all required dependencies for the package.
3. Write the code for the package.
4. Test the code for the package.
5. If you approach TDD methodoloty, write the test code first and then write the code and pass the test.

## Functional Programming
* Distinction between pure and impure code
* Pure functions have no side effects and cannot be mutated and return a value based on only what it was passed 
* Impure functions return unpredictable results (Console.log)

## Higher-order function
* A function that operates on another function
* Return a function (map, filter, reduce)

## Objects & Inheritance
* JS has prototype-based inheritance rather than class-based inheritance
* Slightly different than strictly typed languages
* Anything attached to a prototype is available to use to its descendant
* Using class & extends keywords for ES6 class to use inheritance, it is syntatic sugar for other programming language developer

## Errors
* Important for debugging
* JS has build-in errors, developers allows to write their own error messages 
* Writing good error messages is very important for pinpoint bugs later
  * Timestamp 
  * Message about the problem that occurred
  * Message about the cause of the problem
  * Consistent format so that it can be parsed and searched
  * Severity level (low, med, high) or (0 - 10)

## Handling thrown errors
* Errors can stop code from running
* Use `try{} catch(error){}` to keep code running