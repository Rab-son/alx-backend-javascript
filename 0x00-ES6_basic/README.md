## ES6 Basics
> ES6, also known as ECMAScript 2015, is a version of JavaScript that introduced new syntax and features to the language. In this repository, you'll find information about some of the basics of ES6.

### Getting Started
> To get started with ES6, you'll need to have some basic knowledge of JavaScript programming language. You'll also need to have a browser or a tool that can run JavaScript code with support for ES6 syntax.

### Prerequisites
> Basic knowledge of JavaScript programming language
> A browser or tool that can run JavaScript code with support for ES6 syntax

### Installing
> There's nothing to install to use ES6 syntax in JavaScript. However, if you want to use ES6 syntax in an environment that doesn't support it, such as an older browser, you'll need to use a transpiler like Babel.

### Features
> ES6 introduced many new features to JavaScript, including:

- Arrow Functions
- Template Literals
- Destructuring Assignment
- Rest and Spread Operators
- Classes
- Modules

> Here's an example of how you can use some of these features:

```
// Arrow Function
const greet = name => {
  console.log(`Hello, ${name}!`);
}

// Template Literal
const name = 'John';
greet(name);

// Destructuring Assignment
const person = { name: 'Jane', age: 25 };
const { name, age } = person;
console.log(`${name} is ${age} years old.`);

// Rest and Spread Operators
const numbers = [1, 2, 3, 4, 5];
const sum = (...nums) => nums.reduce((acc, curr) => acc + curr, 0);
console.log(`The sum of ${numbers} is ${sum(...numbers)}.`);

// Classes
class Animal {
  constructor(name) {
    this.name = name;
  }

  speak() {
    console.log(`${this.name} makes a noise.`);
  }
}

class Dog extends Animal {
  constructor(name) {
    super(name);
  }

  speak() {
    console.log(`${this.name} barks.`);
  }
}

const dog = new Dog('Rufus');
dog.speak();

// Modules
import { greet } from './greet.js';
greet('Alice');
```