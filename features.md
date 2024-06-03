# ES6 (ECMAScript 2015) Features 

ES6, also known as ECMAScript 2015, introduced several new features and improvements to JavaScript. Below are some of the notable features:

## Arrow Functions    
The arrow function is a simple  way of writing functions, using the "=>" symbol. This simplifies function expressions and ensures lexical scoping.    

## Classes
ES6 introduced class syntax, providing a more familiar and structured way to create objects and define their behavior, similar to other object-oriented programming languages.
 
## Template Literals
Template literals allow for easier string interpolation and multiline strings, using backticks (`) instead of single or double quotes.

## Destructuring Assignment
A convenient way to extract values from arrays or objects and assign them to variables, making it easier to work with complex data structures.

## Enhanced Object Literals
ES6 introduced shorthand syntax for defining object properties and methods, making object creation and manipulation more concise.

## Modules
A standardized way to organize and share JavaScript code across multiple files, allowing for better code separation and reusability.

## Promises
A built-in mechanism for handling asynchronous operations, providing a more structured and readable way to write asynchronous code compared to callbacks.

## Default Parameters
The ability to define default values for function parameters, ensuring that functions can be called with fewer arguments without causing errors.

## Spread Operator
A concise syntax for expanding arrays or objects into individual elements, making it easier to combine, clone, or manipulate complex data structures.

## Iterators and Generators
ES6 introduced the concept of iterable objects and generators, enabling more powerful and flexible control flow and iteration over data.


### Examples 
code snippets that demonstrate the features of ES6:

1. Classes:
```javascript
class Person {
  constructor(name) {
    this.name = name;
  }
  sayHello() {
    console.log(`Hello, my name is ${this.name}.`);
  }
}

const person = new Person("John");
person.sayHello(); // Output: Hello, my name is John.
```

2. Template Literals:
```javascript
const name = "Alice";
const age = 28;
console.log(`My name is ${name} and I am ${age} years old.`); // Output: My name is Alice and I am 28 years old.
```

3. Destructuring Assignment:
```javascript
const person = {
  name: "John",
  age: 30,
  city: "New York"
};

const { name, age, city } = person;
console.log(name, age, city); // Output: John 30 New York
```

4. Enhanced Object Literals:
```javascript
const name = "Alice";
const age = 28;

const person = {
  name,
  age,
  sayHello() {
    console.log(`Hello, my name is ${this.name}.`);
  }
};

person.sayHello(); // Output: Hello, my name is Alice.
```

5. Modules:
```javascript
// math.js
export const add = (a, b) => a + b;
export const subtract = (a, b) => a - b;

// main.js
import { add, subtract } from './math.js';

console.log(add(5, 3)); // Output: 8
console.log(subtract(5, 3)); // Output: 2
```

6. Promises:
```javascript
const fetchData = () => {
  return new Promise((resolve, reject) => {
    // Simulating an asynchronous API request
    setTimeout(() => {
      const data = "Some data";
      resolve(data);
    }, 2000);
  });
};

fetchData().then((data) => {
  console.log(data); // Output: Some data
});
```

7. Default Parameters:
```javascript
const greet = (name = "Guest") => {
  console.log(`Hello, ${name}!`);
};

greet(); // Output: Hello, Guest!
greet("Alice"); // Output: Hello, Alice!
```

8. Spread Operator:
```javascript
const numbers = [1, 2, 3];
const sum = (a, b, c) => a + b + c;

console.log(sum(...numbers)); // Output: 6
```

9. Iterators and Generators:
```javascript
const myGenerator = function* () {
  yield "Hello";
  yield "World";
};

const generator = myGenerator();

console.log(generator.next().value); // Output: Hello
console.log(generator.next().value); // Output: World
```

### These are the Features of the ES6
