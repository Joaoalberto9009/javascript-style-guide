Evernote Javascript style guide
======================

## Table of Contents

  1. [Strings](#strings)
  2. [Variables](#variables)
  3. [Semicolons](#semicolons)
  4. [Commas](#commas)
  5. [Declaring Strict Mode](#declaring-strict-mode)
  6. [Naming Conventions](#naming-conventions)
  7. [Conditional Expressions](#conditional-expressions)
  8. [Blocks](#Blocks)

## Strings

Use single quotes `''` for strings instead of double quotes `""`

  ```javascript
  // bad
  var name = "Eva Note";

  var fullName = "Eva " + this.lastName;

  // good
  var name = 'Eva Note';

  var fullName = 'Eva ' + this.lastName;
  ```

**[⬆ back to top](#table-of-contents)**


## Variables

Declarations with `var` Always

**[⬆ back to top](#table-of-contents)**


## Semicolons

Use semicolons `;`

  ```javascript
  // bad
  (function() {
    return 'Evernote'
  })();

  // good
  (function() {
    return 'Evernote';
  })();
  ```

**[⬆ back to top](#table-of-contents)**

## Commas

Don's use leading commas.

  ```javascript
  // bad
  var evernote
    , premium
    , business;

  // good
  var evernote,
      premium,
      business;

  // bad
  var product = {
      name: 'Evernote'
    , type: 'App'
    , category: 'Productivity'
  };

  // good
  var product = {
    name: 'Evernote',
    type: 'App',
    category: 'Productivity'
  };

  // good
  (function() {
    return 'Evernote';
  })();
  ```

**[⬆ back to top](#table-of-contents)**

## Naming conventions

  - Use descriptive naming. Avoid single letter names.

  ```javascript
  // bad
  function t() {
    // do something...
  }

  // good
  function test() {
    // do something...
  }
  ```

  - Use camelCase when naming objects, functions, and instances.

  ```javascript
  // bad
  var OBject = {};
  var heres_an_object = {};
  function c() {}
  var u = new user({
    name: 'Evernote';
  });

  // good
  var thisIsMyObject = {};
  function thisIsMyFunction() {}
  var user = new User({
    name: 'Evernote';
  });
  ```

**[⬆ back to top](#table-of-contents)**


## Declaring Strict Mode

Declare `'use strict'` in all your JavaScript files.


**[⬆ back to top](#table-of-contents)**

##Conditional Expressions

Use `===` and `!==`

```javascript
  // bad
  var name = 'Eva Note';
  if(name == 'Eva Note'){}

  if(name != 'Eva Note'){}

  // good
  var name = 'Eva Note';
  if(name === 'Eva Note'){}

  if(name !== 'Eva Note'){}
  ```
**[⬆ back to top](#table-of-contents)**


##Blocks

Use braces when there are multi-line blocks.

```javascript
  // bad
  if (name)
  return false;

  // good
  if (name) return false;

  // bad
  if (name){return false};

  // good
  if (name){
    return false;
  }
  ```
**[⬆ back to top](#table-of-contents)**
