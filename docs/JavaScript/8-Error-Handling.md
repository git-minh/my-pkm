---
sidebar_position: 8
---

### 8. **Error Handling**
- **try...catch...finally**
- **Throwing Errors**

#### **Try...Catch...Finally**
The `try...catch...finally` statement handles errors gracefully in JavaScript.

```javascript
try {
  // Code that might throw an error
  throw new Error("Something went wrong");
} catch (error) {
  // Handle the error
  console.error(error.message);
} finally {
  // Always executed, regardless of error
  console.log("Cleanup code");
}
```

#### **Custom Error Types**
You can create custom error types by extending the Error class.

```javascript
class ValidationError extends Error {
  constructor(message) {
    super(message);
    this.name = "ValidationError";
  }
}

class DatabaseError extends Error {
  constructor(message) {
    super(message);
    this.name = "DatabaseError";
  }
}

// Using custom errors
try {
  throw new ValidationError("Invalid input");
} catch (error) {
  if (error instanceof ValidationError) {
    console.error("Validation Error:", error.message);
  } else if (error instanceof DatabaseError) {
    console.error("Database Error:", error.message);
  } else {
    console.error("Unknown Error:", error.message);
  }
}
```

#### **Error Types**
JavaScript has several built-in error types:

```javascript
// ReferenceError
try {
  console.log(undefinedVariable);
} catch (error) {
  console.error(error.name); // "ReferenceError"
}

// TypeError
try {
  null.toString();
} catch (error) {
  console.error(error.name); // "TypeError"
}

// SyntaxError
try {
  eval("Hello World");
} catch (error) {
  console.error(error.name); // "SyntaxError"
}

// RangeError
try {
  const arr = new Array(-1);
} catch (error) {
  console.error(error.name); // "RangeError"
}
```

#### **Async Error Handling**
Error handling in asynchronous code using promises and async/await.

```javascript
// With Promises
fetchData()
  .then(data => {
    console.log(data);
  })
  .catch(error => {
    console.error("Error fetching data:", error);
  });

// With Async/Await
async function getData() {
  try {
    const data = await fetchData();
    console.log(data);
  } catch (error) {
    console.error("Error fetching data:", error);
  }
}
```

#### **Practical Error Handling Examples**

1. **Form Validation**
```javascript
function validateForm(formData) {
  try {
    if (!formData.username) {
      throw new ValidationError("Username is required");
    }
    if (formData.password.length < 8) {
      throw new ValidationError("Password must be at least 8 characters");
    }
    return true;
  } catch (error) {
    console.error(error.message);
    return false;
  }
}
```

2. **API Error Handling**
```javascript
async function fetchUserData(userId) {
  try {
    const response = await fetch(`/api/users/${userId}`);
    if (!response.ok) {
      throw new Error(`HTTP error! status: ${response.status}`);
    }
    const data = await response.json();
    return data;
  } catch (error) {
    console.error("Error fetching user data:", error);
    throw error; // Re-throw to handle it in the calling function
  }
}
```

3. **Database Operations**
```javascript
class Database {
  async query(sql) {
    try {
      // Simulate database query
      if (!sql) {
        throw new DatabaseError("SQL query is required");
      }
      // Execute query...
    } catch (error) {
      console.error("Database error:", error);
      // Log error to monitoring system
      throw error;
    } finally {
      // Close database connection
      console.log("Closing database connection");
    }
  }
}
```

4. **File Operations**
```javascript
function readFile(path) {
  try {
    // Attempt to read file
    if (!path) {
      throw new Error("File path is required");
    }
    // Read file contents...
  } catch (error) {
    console.error("Error reading file:", error);
    // Provide fallback behavior
    return null;
  }
}
```

5. **Error Handling with Multiple Catches**
```javascript
try {
  const data = await processData();
} catch (error) {
  if (error instanceof NetworkError) {
    // Handle network errors
    console.error("Network error:", error);
  } else if (error instanceof ValidationError) {
    // Handle validation errors
    console.error("Validation error:", error);
  } else {
    // Handle other errors
    console.error("Unknown error:", error);
  }
} finally {
  // Cleanup code
  console.log("Processing completed");
}
``` 