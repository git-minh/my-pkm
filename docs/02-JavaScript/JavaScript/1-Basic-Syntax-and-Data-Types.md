---
sidebar_position: 1
---

### 1. **Basic Syntax and Data Types**
- **Variables:** `var`, `let`, `const`
- **Data Types:** `Number`, `String`, `Boolean`, `Object`, `Array`, `Null`, `Undefined`, `Symbol`, `BigInt`

#### **Variables**
Variables in JavaScript are used to store data values. There are three ways to declare a variable:

- **`var`**: The old way of declaring variables. It has function scope.
- **`let`**: Introduced in ES6, it has block scope.
- **`const`**: Also introduced in ES6, it is used to declare variables whose values cannot be reassigned.

Example:
```javascript
var x = 10; // Function scoped
let y = 20; // Block scoped
const z = 30; // Block scoped and cannot be reassigned
```

#### **Data Types**
JavaScript supports several data types. Here are the primary ones:

1. **Number**: Represents both integer and floating-point numbers.
   ```javascript
   let num = 42;
   let floatNum = 3.14;
   ```

2. **String**: Represents a sequence of characters.
   ```javascript
   let str = "Hello, World!";
   ```

3. **Boolean**: Represents a logical entity and can have two values: `true` and `false`.
   ```javascript
   let isTrue = true;
   let isFalse = false;
   ```

4. **Object**: A collection of key-value pairs.
   ```javascript
   let obj = { name: "John", age: 30 };
   ```

5. **Array**: A list-like structure that can hold multiple values.
   ```javascript
   let arr = [1, 2, 3, 4, 5];
   ```

6. **Null**: Represents the intentional absence of any object value.
   ```javascript
   let emptyValue = null;
   ```

7. **Undefined**: Indicates that a variable has not been assigned a value.
   ```javascript
   let notAssigned;
   ```

8. **Symbol**: A unique and immutable primitive value.
   ```javascript
   let sym = Symbol("unique");
   ```

9. **BigInt**: Represents whole numbers larger than `2^53 - 1`.
   ```javascript
   let bigNumber = 1234567890123456789012345678901234567890n;
   ``` 