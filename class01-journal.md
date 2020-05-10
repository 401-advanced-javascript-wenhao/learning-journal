# Class 1 - Program introduction, Node Ecosystem, TDD, CI/CD - 4/13/2020

## Program Introduction - Advanced SD in Full-Stack JS
* Training Period: 4/13/2020-6/19/2020, M-F, 09:00-18:00
* Instructor: Brian Nations, brian@codefellows.com
* Canvas: https://canvas.instructure.com/courses/1907667
* Class Logistics
  * Zoom Lectures - https://zoom.us/j/91562445831
  * Remo Lab - https://live.remo.co/e/code-fellows-labtime

## Node.js
* Open source framework with V8 javascript runtime engine
* Asynchronous and Non-Block
* Use an event loop to run asynchronous I/O with ease

## package.json
* Configures a Node.js package
* Contains meta data and dependencies information
* Run `npm init -y` to initiate package.json file
* Run `npm install` to install dependencies that required for the package
* Run `npm install package_name` to install specific dependency

## CommonJS Modules
* Organizes and modularize code into smaller files
* This is key to scalability
* Use `module.exports` to make code accessible to another modules
* Use `require` or `import` to import a module

## Test Driven Development (TDD)
* A methodology for writing code - write the test first
* Speeds up development cycle and validates integrity of new code and understand goals
  * RED: plan code and write tests for expected behavior that should fail
  * GREEN: write code to pass tests, don't focus on optimization
  * REFACTOR: optimize code for speed, memory, and legibility

## Continuous Integration (CI)
* Process of regularly merging individual features
* Works well with automated tests, code reviews, testing support etc.

## Continuous Delivery (CD)
* Deploying in short cycles
* Code always ready to deploy
* Often paired with CI to enforce stability

## Github Actions
* Github Actions is a CI system that provided by Github
* It is handled via rules defined in `.yml` file in the `.github/workspaces` directory in the root directory of repo
* Github will automatically run tests on PUSH/PR, enforces tests passing to merge

## Node Package Manager (NPM)
* Allows developers to publish packages for others to use
* Be used internally to re-use code across projects
* Use npm client locally to upload/download on the NPM website

## Jest
* Test runner for JS
* Can use `Babel` to convert JS code to browser-compatible JS
* Support typeScript and other features