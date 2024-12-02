---
sidebar_position: 2
---

### 2. **Operators**
- **Arithmetic Operators:** `+`, `-`, `*`, `/`, `%`
- **Comparison Operators:** `==`, `===`, `!=`, `!==`, `>`, `<`, `>=`, `<=`
- **Logical Operators:** `&&`, `||`, `!`
- **Assignment Operators:** `=`, `+=`, `-=`, `*=`, `/=`
- **Ternary Operator:** `condition ? expr1 : expr2`

#### **Arithmetic Operators**
These operators are used to perform mathematical calculations.

- **Addition (`+`)**: Adds two values.
  ```javascript
  let sum = 5 + 3; // 8
  ```

- **Subtraction (`-`)**: Subtracts one value from another.
  ```javascript
  let difference = 5 - 3; // 2
  ```

- **Multiplication (`*`)**: Multiplies two values.
  ```javascript
  let product = 5 * 3; // 15
  ```

- **Division (`/`)**: Divides one value by another.
  ```javascript
  let quotient = 6 / 3; // 2
  ```

- **Modulus (`%`)**: Returns the remainder of a division.
  ```javascript
  let remainder = 7 % 3; // 1
  ```

#### **Comparison Operators**
These operators compare two values and return a Boolean (`true` or `false`).

- **Equal (`==`)**: Checks if two values are equal (type conversion may occur).
  ```javascript
  let isEqual = (5 == '5'); // true
  ```

- **Strict Equal (`===`)**: Checks if two values are equal and of the same type.
  ```javascript
  let isStrictEqual = (5 === '5'); // false
  ```

- **Not Equal (`!=`)**: Checks if two values are not equal.
  ```javascript
  let isNotEqual = (5 != '5'); // false
  ```

- **Strict Not Equal (`!==`)**: Checks if two values are not equal and/or not of the same type.
  ```javascript
  let isStrictNotEqual = (5 !== '5'); // true
  ```

#### **Logical Operators**
These operators are used to combine multiple Boolean expressions.

- **AND (`&&`)**: Returns `true` if both operands are true.
  ```javascript
  let andResult = (5 > 3 && 2 < 4); // true
  ```

- **OR (`||`)**: Returns `true` if at least one operand is true.
  ```javascript
  let orResult = (5 > 3 || 2 > 4); // true
  ```

- **NOT (`!`)**: Returns the inverse of a Boolean value.
  ```javascript
  let notResult = !(5 > 3); // false
  ```

#### **Assignment Operators**
These operators assign values to variables.

- **Assignment (`=`)**: Assigns a value to a variable.
  ```javascript
  let x = 5;
  ```

- **Addition Assignment (`+=`)**: Adds and assigns.
  ```javascript
  let x = 5;
  x += 3; // x = 8
  ```

- **Subtraction Assignment (`-=`)**: Subtracts and assigns.
  ```javascript
  let x = 5;
  x -= 3; // x = 2
  ```

#### **Ternary Operator**
A shorthand for the `if...else` statement.

```javascript
let age = 18;
let canVote = (age >= 18) ? "Yes" : "No"; // "Yes"
``` 