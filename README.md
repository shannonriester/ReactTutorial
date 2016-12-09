# React

## State
  1. State updates may be asynch...
    **PreviousState**
      ```js
      this.setState((prevState, props) => {
        counter: prevState.counter + props.increment,
      });    
      ```
  2. State updates are merged     

## React DOM
  - Only re-renders the specific part of an Element that changes

## Elements
  - Immutable. Cannot change its children or attributes
  - User-defined components `<Modal name="Shannon"/>`

## ES6  
  - **Classes**
    - special _functions_
      - Two components
      1. Expressions
        ```js
        // unnamed
        var Polygon = class {
          constructor(height, width) {
            this.height = height;
            this.width = width;
          }
        };

        // named
        var Polygon = class Polygon {
          constructor(height, width) {
            this.height = height;
            this.width = width;
          }
        };        
        ```
      2. Declarations
        - NOT hoisted (unlike functions)
        ```js
        class Polygon {
          constructor(height, width) {
            this.height = height;
            this.width = width;
          }
        }

        ```
    - prototype-based inheritance
    - `constructor()` method creates and initializes an object created with a class
  **Super(props)**
    - Used to call functions on an object's parent
    - `super.functionOnParent([arguments]);`
    - ex: `super.hideModal(username, password);`


# Basic Build with NPM scripts
This is a project scaffolding and build tool for the TIY Austin Front-End Engineering course. Feel free to use and enjoy! Feedback and PRs welcome!

## Features
- es2015 and babel, including module syntax
- mocha test runner
- sass (.scss)

## Installation
- Clone this repo (or fork then clone, if you prefer)
- Remove the git history by running `rm -rf .git`
- Set up a new git repo
- Run `npm install`
- if you get permission errors you may need to run `sudo npm install` to install a couple global dependencies

## Use
- `npm install` will scaffold your project AND start the dev server
- `npm start` will start the dev server and watch for changes
- `npm test` will run any test files included in the test folder
- When the server is running, your site will be live on [http://localhost:8080/](http://localhost:8080/)

## Dependencies
- `sass` [install guide here](http://sass-lang.com/install)
