---
sidebar_position: 6
---

### 6. **Scope and Closures**
- **Global Scope**
- **Local Scope**
- **Block Scope**
- **Closures and Lexical Scoping**

#### **Scope**
Scope determines the accessibility of variables and functions in your code.

1. **Global Scope**
   Variables declared outside any function are in the global scope.
   ```javascript
   const globalVar = "I am global";

   function test() {
     console.log(globalVar); // Can access global variable
   }

   test();
   console.log(globalVar); // Can access global variable
   ```

2. **Local Scope (Function Scope)**
   Variables declared inside a function are only accessible within that function.
   ```javascript
   function test() {
     const localVar = "I am local";
     console.log(localVar); // Can access local variable
   }

   test();
   // console.log(localVar); // Error: localVar is not defined
   ```

3. **Block Scope**
   Variables declared with `let` and `const` are block-scoped.
   ```javascript
   if (true) {
     let blockVar = "I am block-scoped";
     const alsoBlockScoped = "Me too";
     console.log(blockVar); // Can access within block
   }
   // console.log(blockVar); // Error: blockVar is not defined
   ```

#### **Closures**
A closure is a function that has access to variables in its outer (enclosing) lexical scope, even after the outer function has returned.

1. **Basic Closure**
   ```javascript
   function outer() {
     const message = "Hello";
     
     function inner() {
       console.log(message); // Can access message from outer scope
     }
     
     return inner;
   }

   const sayHello = outer();
   sayHello(); // Output: Hello
   ```

2. **Practical Use of Closures**
   ```javascript
   // Counter with private variable
   function createCounter() {
     let count = 0;
     
     return {
       increment() {
         count++;
         console.log(count);
       },
       decrement() {
         count--;
         console.log(count);
       },
       getCount() {
         return count;
       }
     };
   }

   const counter = createCounter();
   counter.increment(); // Output: 1
   counter.increment(); // Output: 2
   counter.decrement(); // Output: 1
   console.log(counter.getCount()); // Output: 1
   ```

3. **Factory Functions with Closures**
   ```javascript
   function createPerson(name) {
     let age = 0;
     
     return {
       getName() {
         return name;
       },
       setAge(newAge) {
         age = newAge;
       },
       getAge() {
         return age;
       }
     };
   }

   const person = createPerson("John");
   person.setAge(30);
   console.log(person.getName()); // Output: John
   console.log(person.getAge()); // Output: 30
   ```

4. **Module Pattern**
   ```javascript
   const calculator = (function() {
     let result = 0;
     
     return {
       add(x) {
         result += x;
         return this;
       },
       subtract(x) {
         result -= x;
         return this;
       },
       getResult() {
         return result;
       }
     };
   })();

   calculator.add(5).subtract(2);
   console.log(calculator.getResult()); // Output: 3
   ```

5. **Event Handlers with Closures**
   ```javascript
   function setupHandler(element, event, callback) {
     element.addEventListener(event, function() {
       callback(element);
     });
   }

   setupHandler(button, "click", function(element) {
     console.log("Button clicked:", element.id);
   });
   ```

#### **Lexical Scoping**
JavaScript uses lexical scoping, which means that the scope of a variable is determined by its location within the source code.

```javascript
const x = 10;

function outer() {
  const y = 20;
  
  function inner() {
    const z = 30;
    console.log(x, y, z); // Can access all variables
  }
  
  inner();
}

outer(); // Output: 10 20 30
``` 