---
sidebar_position: 4
---

### 4. **Functions**
- **Function Declaration:** `function myFunction() {}`
- **Function Expression:** `const myFunction = function() {}`
- **Arrow Functions:** `const myFunction = () => {}`
- **Parameters and Arguments**
- **Return Values**

#### **Function Declaration**
A function declaration defines a named function.

```javascript
function greet(name) {
  return "Hello, " + name + "!";
}

console.log(greet("John")); // Output: Hello, John!
```

#### **Function Expression**
A function expression defines a function as part of a larger expression.

```javascript
const greet = function(name) {
  return "Hello, " + name + "!";
};

console.log(greet("John")); // Output: Hello, John!
```

#### **Arrow Functions**
Arrow functions provide a shorter syntax for writing function expressions.

```javascript
const greet = (name) => {
  return "Hello, " + name + "!";
};

// For single expressions, you can omit the return statement and curly braces
const greetShort = name => "Hello, " + name + "!";

console.log(greet("John")); // Output: Hello, John!
console.log(greetShort("John")); // Output: Hello, John!
```

#### **Parameters and Arguments**
Functions can take parameters (variables listed in function definition) and arguments (values passed to the function).

```javascript
// Function with multiple parameters
function add(a, b) {
  return a + b;
}

console.log(add(5, 3)); // Output: 8

// Default parameters
function greet(name = "Guest") {
  return "Hello, " + name + "!";
}

console.log(greet()); // Output: Hello, Guest!
console.log(greet("John")); // Output: Hello, John!

// Rest parameters
function sum(...numbers) {
  return numbers.reduce((total, num) => total + num, 0);
}

console.log(sum(1, 2, 3, 4)); // Output: 10
```

#### **Return Values**
Functions can return values using the `return` statement.

```javascript
function multiply(a, b) {
  return a * b;
}

const result = multiply(4, 5);
console.log(result); // Output: 20

// Early return
function isPositive(number) {
  if (number <= 0) {
    return false;
  }
  return true;
}

console.log(isPositive(5)); // Output: true
console.log(isPositive(-3)); // Output: false
```

#### **Callback Functions**
Functions that are passed as arguments to other functions.

```javascript
function processUserInput(callback) {
  const name = "John";
  callback(name);
}

function greet(name) {
  console.log("Hello, " + name + "!");
}

processUserInput(greet); // Output: Hello, John!
```

#### **Immediately Invoked Function Expression (IIFE)**
A function that runs as soon as it is defined.

```javascript
(function() {
  console.log("This function runs immediately!");
})();

// IIFE with parameters
(function(name) {
  console.log("Hello, " + name + "!");
})("John");
``` 