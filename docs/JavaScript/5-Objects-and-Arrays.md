---
sidebar_position: 5
---

### 5. **Objects and Arrays**
- **Object Literals:** `{ key: value }`
- **Array Methods:** `push()`, `pop()`, `shift()`, `unshift()`, `map()`, `filter()`, `reduce()`, `forEach()`, `find()`, `includes()`

#### **Objects**
Objects are collections of key-value pairs.

```javascript
// Creating an object
const person = {
  name: "John",
  age: 30,
  isStudent: false,
  greet: function() {
    return "Hello, my name is " + this.name;
  }
};

// Accessing object properties
console.log(person.name); // Output: John
console.log(person["age"]); // Output: 30

// Adding new properties
person.country = "USA";

// Modifying properties
person.age = 31;

// Deleting properties
delete person.isStudent;

// Object methods
console.log(person.greet()); // Output: Hello, my name is John
```

#### **Arrays**
Arrays are ordered collections of values.

```javascript
// Creating an array
const fruits = ["apple", "banana", "orange"];

// Accessing array elements
console.log(fruits[0]); // Output: apple

// Modifying array elements
fruits[1] = "grape";

// Array length
console.log(fruits.length); // Output: 3
```

#### **Array Methods**

1. **`push()` and `pop()`**
   ```javascript
   const numbers = [1, 2, 3];
   
   // push: Add to end
   numbers.push(4);
   console.log(numbers); // Output: [1, 2, 3, 4]
   
   // pop: Remove from end
   const lastNumber = numbers.pop();
   console.log(lastNumber); // Output: 4
   console.log(numbers); // Output: [1, 2, 3]
   ```

2. **`shift()` and `unshift()`**
   ```javascript
   const numbers = [1, 2, 3];
   
   // unshift: Add to beginning
   numbers.unshift(0);
   console.log(numbers); // Output: [0, 1, 2, 3]
   
   // shift: Remove from beginning
   const firstNumber = numbers.shift();
   console.log(firstNumber); // Output: 0
   console.log(numbers); // Output: [1, 2, 3]
   ```

3. **`map()`**
   ```javascript
   const numbers = [1, 2, 3];
   const doubled = numbers.map(num => num * 2);
   console.log(doubled); // Output: [2, 4, 6]
   ```

4. **`filter()`**
   ```javascript
   const numbers = [1, 2, 3, 4, 5];
   const evenNumbers = numbers.filter(num => num % 2 === 0);
   console.log(evenNumbers); // Output: [2, 4]
   ```

5. **`reduce()`**
   ```javascript
   const numbers = [1, 2, 3, 4];
   const sum = numbers.reduce((acc, curr) => acc + curr, 0);
   console.log(sum); // Output: 10
   ```

6. **`forEach()`**
   ```javascript
   const fruits = ["apple", "banana", "orange"];
   fruits.forEach(fruit => console.log(fruit));
   // Output:
   // apple
   // banana
   // orange
   ```

7. **`find()`**
   ```javascript
   const numbers = [1, 2, 3, 4, 5];
   const firstEven = numbers.find(num => num % 2 === 0);
   console.log(firstEven); // Output: 2
   ```

8. **`includes()`**
   ```javascript
   const fruits = ["apple", "banana", "orange"];
   console.log(fruits.includes("banana")); // Output: true
   console.log(fruits.includes("grape")); // Output: false
   ```

#### **Combining Objects and Arrays**

```javascript
// Array of objects
const users = [
  { id: 1, name: "John", age: 30 },
  { id: 2, name: "Jane", age: 25 },
  { id: 3, name: "Bob", age: 35 }
];

// Finding objects in array
const user = users.find(user => user.id === 2);
console.log(user); // Output: { id: 2, name: "Jane", age: 25 }

// Filtering objects
const adults = users.filter(user => user.age >= 30);
console.log(adults); // Output: [{ id: 1, name: "John", age: 30 }, { id: 3, name: "Bob", age: 35 }]

// Mapping objects
const names = users.map(user => user.name);
console.log(names); // Output: ["John", "Jane", "Bob"]
``` 