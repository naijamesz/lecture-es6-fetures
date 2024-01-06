# lecture-es6-fetures EN
## ES6 Features

ES6 or ECMAScript 2015 is a significant update for JavaScript, introducing many new features to make coding easier and more efficient. Here is a summary of the main features in ES6 along with examples of how to use them:

1. **Let and Const**

   - `let` is used to declare variables that can be reassigned.
   - `const` is used to declare variables with constant values.
   - Example:
     ```javascript
     let name = 'Alice';
     const PI = 3.14;
     ```

2. **Arrow Functions**

   - Arrow functions provide a more concise syntax for defining functions.
   - Example:
     ```javascript
     const add = (a, b) => a + b;
     ```

3. **Template Literals**

   - Template literals use backticks (`` ` ``) to create strings that can include variables and multiline expressions.
   - Example:
     ```javascript
     let name = 'Bob';
     console.log(`Hello, ${name}!`);
     ```

4. **Destructuring Assignment**

   - Destructuring assignment provides an easy way to extract values from arrays or properties from objects.
   - Example:
     ```javascript
     const [a, b] = [1, 2];
     const { x, y } = { x: 10, y: 20 };
     ```

5. **Default Parameters**

   - Default parameters allow you to specify default values for function parameters.
   - Example:
     ```javascript
     function greet(name = 'Guest') {
       console.log(`Hello, ${name}!`);
     }
     ```

6. **Import/Export Modules**

   - Modules allow you to split your code into separate files and import or export functions, classes, or variables.
   - Example:

     ```javascript
     // file math.js
     export const add = (a, b) => a + b;

     // file main.js
     import { add } from './math.js';
     console.log(add(2, 3));
     ```

7. **Promises and Async/Await**

   - Promises and async/await provide a way to handle asynchronous operations.
   - Example:
     ```javascript
     const fetchData = async () => {
       try {
         let response = await fetch('https://api.example.com/data');
         let data = await response.json();
         console.log(data);
       } catch (error) {
         console.error('Error:', error);
       }
     };
     ```

8. **Classes**

   - Classes provide a new syntax for creating objects and managing inheritance.
   - Example:
     ```javascript
     class Person {
       constructor(name) {
         this.name = name;
       }
       greet() {
         console.log(`Hello, my name is ${this.name}`);
       }
     }
     ```

9. **New Built-in Methods**

   - New methods for objects, arrays, etc.
   - Example:
     ```javascript
     Object.assign({}, { x: 1, y: 2 }); // {x: 1, y: 2}
     Array.from('foo'); // ['f', 'o', 'o']
     ```

10. **Spread/Rest Operator**

    - The `...` operator is used to spread the elements of an array or object or gather parameters in a function.
    - Example:

      ```javascript
      const numbers = [1, 2, 3];
      const moreNumbers = [...numbers, 4, 5]; // [1, 2, 3, 4, 5]

      function sum(...args) {
        return args.reduce((acc, current) => acc + current, 0);
      }
      ```

ES6 introduces features that make JavaScript more capable and flexible, paving the way for future JavaScript development.
