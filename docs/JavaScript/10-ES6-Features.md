---
sidebar_position: 10
---

### 10. **ES6+ Features**
- **Template Literals:** `` `Hello, ${name}` ``
- **Destructuring:** `{ key } = object`, `[first, second] = array`
- **Spread Operator:** `...array`
- **Rest Parameters:** `function(...args) {}`
- **Modules:** `import`, `export`
- **Default Parameters**

#### **Template Literals**
Template literals allow embedded expressions and multi-line strings.

```javascript
const name = "John";
const greeting = `Hello, ${name}!`;

// Multi-line strings
const multiLine = `
  This is a
  multi-line
  string
`;
```

#### **Destructuring**
Destructuring allows unpacking values from arrays or properties from objects.

```javascript
// Array Destructuring
const numbers = [1, 2, 3];
const [first, second, third] = numbers;

// Object Destructuring
const person = { name: "John", age: 30 };
const { name, age } = person;

// With Default Values
const { name: userName = "Guest" } = {};

// Nested Destructuring
const user = {
  id: 1,
  details: {
    firstName: "John",
    lastName: "Doe"
  }
};
const { details: { firstName, lastName } } = user;
```

#### **Spread Operator**
The spread operator expands arrays or objects.

```javascript
// Array Spread
const arr1 = [1, 2, 3];
const arr2 = [...arr1, 4, 5];

// Object Spread
const obj1 = { foo: "bar", x: 42 };
const obj2 = { ...obj1, y: 13 };

// Function Arguments
const numbers = [1, 2, 3];
console.log(Math.max(...numbers));

// Array Copy
const original = [1, 2, 3];
const copy = [...original];

// Merge Objects
const defaults = { theme: "dark", lang: "en" };
const userPrefs = { theme: "light" };
const settings = { ...defaults, ...userPrefs };
```

#### **Rest Parameters**
Rest parameters allow representing an indefinite number of arguments as an array.

```javascript
function sum(...numbers) {
  return numbers.reduce((total, num) => total + num, 0);
}

console.log(sum(1, 2, 3, 4)); // 10

// With other parameters
function multiply(multiplier, ...numbers) {
  return numbers.map(num => multiplier * num);
}

console.log(multiply(2, 1, 2, 3)); // [2, 4, 6]
```

#### **Modules**
Modules allow splitting code into separate files.

```javascript
// math.js
export const add = (a, b) => a + b;
export const subtract = (a, b) => a - b;
export default class Calculator {
  multiply(a, b) {
    return a * b;
  }
}

// main.js
import Calculator, { add, subtract } from './math.js';

console.log(add(2, 3)); // 5
console.log(subtract(5, 2)); // 3

const calc = new Calculator();
console.log(calc.multiply(2, 3)); // 6
```

#### **Default Parameters**
Default parameters allow parameters to have default values if no argument is passed.

```javascript
function greet(name = "Guest", greeting = "Hello") {
  return `${greeting}, ${name}!`;
}

console.log(greet()); // "Hello, Guest!"
console.log(greet("John")); // "Hello, John!"
console.log(greet("John", "Hi")); // "Hi, John!"
```

#### **Other ES6+ Features**

1. **Arrow Functions**
```javascript
const add = (a, b) => a + b;
const square = x => x * x;
const logger = () => console.log("Hello!");
```

2. **Classes**
```javascript
class Person {
  constructor(name) {
    this.name = name;
  }

  greet() {
    return `Hello, I'm ${this.name}`;
  }

  static create(name) {
    return new Person(name);
  }
}
```

3. **Enhanced Object Literals**
```javascript
const name = "John";
const age = 30;

const person = {
  name,
  age,
  greet() {
    return `Hello, I'm ${this.name}`;
  }
};
```

4. **Map and Set**
```javascript
// Map
const map = new Map();
map.set("key", "value");
map.get("key");

// Set
const set = new Set([1, 2, 3, 3]);
console.log([...set]); // [1, 2, 3]
```

5. **Promises and Async/Await**
```javascript
// Promise
const promise = new Promise((resolve, reject) => {
  setTimeout(() => resolve("Done!"), 1000);
});

// Async/Await
async function fetchData() {
  try {
    const response = await fetch('https://api.example.com/data');
    const data = await response.json();
    return data;
  } catch (error) {
    console.error('Error:', error);
  }
}
```

6. **Optional Chaining**
```javascript
const user = {
  details: {
    name: "John"
  }
};

console.log(user?.details?.name); // "John"
console.log(user?.address?.street); // undefined
```

7. **Nullish Coalescing**
```javascript
const value = null;
const defaultValue = "default";

console.log(value ?? defaultValue); // "default"
``` 