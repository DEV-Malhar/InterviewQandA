Here are 10 JavaScript technical interview questions along with sample answers for someone with 3 years of developer experience:

1. **What are the key differences between `let`, `const`, and `var` in JavaScript?**
   - `var` is function-scoped and can be redeclared and reassigned.
   - `let` is block-scoped, can be reassigned but not redeclared.
   - `const` is block-scoped and cannot be redeclared or reassigned.

2. **Explain the concept of hoisting in JavaScript.**
   - Hoisting is a JavaScript mechanism where variable and function declarations are moved to the top of their containing scope during compilation, before the code is executed.

3. **What is closure in JavaScript? Provide an example.**
   - A closure is a function that has access to its own scope, as well as the scope in which it was created. It allows functions to retain access to variables from their containing scopes even after the outer function has finished executing.
   ```javascript
   function outerFunction() {
       let outerVariable = 'I am outer';
       function innerFunction() {
           console.log(outerVariable);
       }
       return innerFunction;
   }
   let inner = outerFunction();
   inner(); // Output: I am outer
   ```

4. **How does prototypal inheritance work in JavaScript?**
   - In JavaScript, objects can inherit properties and methods from other objects through the prototype chain. Each object has a prototype object from which it inherits properties. If a property or method is not found on an object, JavaScript looks up the prototype chain until it finds the property or until it reaches the end of the chain (Object.prototype).

5. **Explain the difference between `==` and `===` in JavaScript.**
   - `==` is an equality operator that performs type coercion, meaning it converts the operands to the same type before comparing them. `===` is a strict equality operator that does not perform type coercion and checks both the value and the type of the operands.

6. **What are the different ways to create objects in JavaScript?**
   - There are several ways to create objects in JavaScript, including object literals, constructor functions, the `Object.create()` method, and ES6 classes.

7. **What is event delegation in JavaScript?**
   - Event delegation is a technique where a single event listener is attached to a parent element, rather than multiple event listeners being attached to individual child elements. This allows you to handle events for multiple elements with a single event listener, improving performance and reducing memory usage.

8. **Explain the difference between `null` and `undefined` in JavaScript.**
   - `null` represents the intentional absence of any value and is often used to indicate that a variable has been explicitly set to "nothing". `undefined` is used to represent an uninitialized or missing value and is the default value for variables that have not been assigned a value.

9. **What are promises in JavaScript? Provide an example of how to use them.**
   - Promises are objects that represent the eventual completion or failure of an asynchronous operation. They allow you to write asynchronous code in a more readable and manageable way. Here's an example:
   ```javascript
   function fetchData() {
       return new Promise((resolve, reject) => {
           // Simulate an asynchronous operation
           setTimeout(() => {
               resolve('Data fetched successfully');
           }, 2000);
       });
   }
   fetchData().then((data) => {
       console.log(data); // Output: Data fetched successfully
   });
   ```

10. **How does the `this` keyword work in JavaScript?**
    - The `this` keyword refers to the object that is executing the current function. The value of `this` is determined by how a function is called, rather than where it is defined. In the global scope or inside a function, `this` refers to the global object (e.g., `window` in browsers, `global` in Node.js). In a method, `this` refers to the object that owns the method.

These answers should help you prepare for a JavaScript technical interview and demonstrate your expertise with 3 years of developer experience.

>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>> JSON >>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
Here are 10 JSON technical interview questions along with sample answers for someone with 3 years of developer experience:

1. **What is JSON?**
   - JSON (JavaScript Object Notation) is a lightweight data-interchange format that is easy for humans to read and write and easy for machines to parse and generate. It is based on JavaScript syntax, but it is language-independent.

2. **What are the basic data types in JSON?**
   - JSON supports six basic data types: string, number, object, array, boolean, and null.

3. **How do you parse JSON data in JavaScript?**
   - In JavaScript, you can parse JSON data using the `JSON.parse()` method, which converts a JSON string into a JavaScript object.

4. **What is the difference between JSON and XML?**
   - JSON is more lightweight and easier to read and write than XML. JSON is also more efficient to parse and generate than XML. However, JSON does not support as many data types and is less suitable for hierarchical data structures than XML.

5. **How do you stringify an object in JavaScript to convert it into JSON format?**
   - In JavaScript, you can stringify an object into JSON format using the `JSON.stringify()` method, which converts a JavaScript object into a JSON string.

6. **How do you handle nested objects in JSON?**
   - Nested objects in JSON are represented by placing one object inside another object. For example:
     ```json
     {
       "name": "John Doe",
       "age": 30,
       "address": {
         "street": "123 Main St",
         "city": "Anytown"
       }
     }
     ```

7. **How do you validate JSON data?**
   - JSON data can be validated using JSON Schema, which is a vocabulary that allows you to annotate and validate JSON documents.

8. **What is JSONP and how does it work?**
   - JSONP (JSON with Padding) is a technique for making cross-domain AJAX requests by using a `<script>` tag to load JSON data from a different domain. It works by wrapping the JSON data in a callback function specified by the client.

9. **How do you handle errors when parsing JSON data in JavaScript?**
   - When parsing JSON data in JavaScript, you can use a `try-catch` block to handle errors that may occur during parsing. For example:
     ```javascript
     try {
       var data = JSON.parse(jsonString);
     } catch (e) {
       console.error("Error parsing JSON: " + e.message);
     }
     ```

10. **How do you pretty-print JSON data for better readability?**
    - In JavaScript, you can use the `JSON.stringify()` method with the optional `space` parameter to pretty-print JSON data. For example:
      ```javascript
      var data = { "name": "John Doe", "age": 30 };
      var prettyJson = JSON.stringify(data, null, 2);
      console.log(prettyJson);
      ```

These answers should help you prepare for a JSON technical interview and demonstrate your expertise with 3 years of developer experience.