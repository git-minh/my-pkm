---
sidebar_position: 3
---

### 3. **Control Structures**
- **Conditional Statements:** `if`, `else if`, `else`, `switch`
- **Loops:** `for`, `while`, `do...while`, `for...in`, `for...of`

#### **Conditional Statements**

1. **`if` Statement**
   The `if` statement executes a block of code if a specified condition is true.

   ```javascript
   let age = 18;
   if (age >= 18) {
     console.log("You are an adult.");
   }
   ```

2. **`else if` Statement**
   The `else if` statement specifies a new condition to test if the first condition is false.

   ```javascript
   let age = 16;
   if (age >= 18) {
     console.log("You are an adult.");
   } else if (age >= 13) {
     console.log("You are a teenager.");
   }
   ```

3. **`else` Statement**
   The `else` statement executes a block of code if all previous conditions are false.

   ```javascript
   let age = 10;
   if (age >= 18) {
     console.log("You are an adult.");
   } else if (age >= 13) {
     console.log("You are a teenager.");
   } else {
     console.log("You are a child.");
   }
   ```

4. **`switch` Statement**
   The `switch` statement executes different code blocks based on different conditions.

   ```javascript
   let day = 2;
   switch (day) {
     case 1:
       console.log("Monday");
       break;
     case 2:
       console.log("Tuesday");
       break;
     case 3:
       console.log("Wednesday");
       break;
     default:
       console.log("Invalid day");
   }
   ```

#### **Loops**

1. **`for` Loop**
   The `for` loop repeats a block of code a specified number of times.

   ```javascript
   for (let i = 0; i < 5; i++) {
     console.log(i); // 0, 1, 2, 3, 4
   }
   ```

2. **`while` Loop**
   The `while` loop repeats a block of code while a specified condition is true.

   ```javascript
   let i = 0;
   while (i < 5) {
     console.log(i); // 0, 1, 2, 3, 4
     i++;
   }
   ```

3. **`do...while` Loop**
   The `do...while` loop executes a block of code once before checking the condition.

   ```javascript
   let i = 0;
   do {
     console.log(i); // 0, 1, 2, 3, 4
     i++;
   } while (i < 5);
   ```

4. **`for...in` Loop**
   The `for...in` loop iterates over the properties of an object.

   ```javascript
   let person = { name: "John", age: 30 };
   for (let key in person) {
     console.log(key + ": " + person[key]);
   }
   ```

5. **`for...of` Loop**
   The `for...of` loop iterates over iterable objects like arrays.

   ```javascript
   let numbers = [1, 2, 3];
   for (let num of numbers) {
     console.log(num);
   }
   ``` 