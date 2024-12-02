---
sidebar_position: 7
---

### 7. **Asynchronous JavaScript**
- **Callbacks**
- **Promises:** `.then()`, `.catch()`, `.finally()`
- **Async/Await**

#### **Callbacks**
A callback is a function passed as an argument to another function, which is executed after the main function has finished its execution.

```javascript
// Simple callback example
function fetchData(callback) {
  setTimeout(() => {
    const data = { id: 1, name: "John" };
    callback(data);
  }, 1000);
}

fetchData((data) => {
  console.log(data); // Output after 1 second: { id: 1, name: "John" }
});

// Callback hell example (problematic)
fetchUserData((user) => {
  fetchUserPosts(user.id, (posts) => {
    fetchPostComments(posts[0].id, (comments) => {
      console.log(comments);
    });
  });
});
```

#### **Promises**
Promises provide a more elegant way to handle asynchronous operations.

```javascript
// Creating a promise
const myPromise = new Promise((resolve, reject) => {
  const success = true;
  
  if (success) {
    resolve("Operation successful");
  } else {
    reject("Operation failed");
  }
});

// Using promises
myPromise
  .then(result => console.log(result))
  .catch(error => console.error(error))
  .finally(() => console.log("Promise completed"));

// Chaining promises
function fetchUser(id) {
  return new Promise((resolve, reject) => {
    setTimeout(() => {
      const user = { id: id, name: "John" };
      resolve(user);
    }, 1000);
  });
}

function fetchUserPosts(userId) {
  return new Promise((resolve, reject) => {
    setTimeout(() => {
      const posts = [
        { id: 1, title: "Post 1" },
        { id: 2, title: "Post 2" }
      ];
      resolve(posts);
    }, 1000);
  });
}

fetchUser(1)
  .then(user => fetchUserPosts(user.id))
  .then(posts => console.log(posts))
  .catch(error => console.error(error));

// Promise.all
const promise1 = Promise.resolve(3);
const promise2 = new Promise(resolve => setTimeout(() => resolve(42), 1000));

Promise.all([promise1, promise2])
  .then(values => console.log(values)); // Output after 1 second: [3, 42]
```

#### **Async/Await**
Async/await provides a more synchronous way to write asynchronous code.

```javascript
// Basic async/await
async function fetchData() {
  try {
    const response = await fetch('https://api.example.com/data');
    const data = await response.json();
    console.log(data);
  } catch (error) {
    console.error('Error:', error);
  }
}

// Sequential async/await
async function fetchUserAndPosts(userId) {
  try {
    const user = await fetchUser(userId);
    const posts = await fetchUserPosts(user.id);
    return posts;
  } catch (error) {
    console.error('Error:', error);
  }
}

// Parallel async/await with Promise.all
async function fetchMultipleUsers(userIds) {
  try {
    const userPromises = userIds.map(id => fetchUser(id));
    const users = await Promise.all(userPromises);
    return users;
  } catch (error) {
    console.error('Error:', error);
  }
}

// Practical example
async function fetchGitHubUser(username) {
  try {
    const response = await fetch(`https://api.github.com/users/${username}`);
    if (!response.ok) {
      throw new Error('User not found');
    }
    const data = await response.json();
    return data;
  } catch (error) {
    console.error('Error:', error);
    throw error;
  }
}

// Using async function
async function displayUserInfo() {
  try {
    const user = await fetchGitHubUser('octocat');
    console.log(`Name: ${user.name}`);
    console.log(`Followers: ${user.followers}`);
  } catch (error) {
    console.error('Failed to fetch user:', error);
  }
}

displayUserInfo();
```

#### **Error Handling in Async Code**

```javascript
// With Promises
fetchData()
  .then(result => {
    // Handle success
    console.log(result);
  })
  .catch(error => {
    // Handle error
    console.error('Error:', error);
  })
  .finally(() => {
    // Always executed
    console.log('Operation completed');
  });

// With Async/Await
async function handleData() {
  try {
    const result = await fetchData();
    console.log(result);
  } catch (error) {
    console.error('Error:', error);
  } finally {
    console.log('Operation completed');
  }
}
```

#### **Real-world Example: Loading Data with Loading State**

```javascript
class DataLoader {
  constructor() {
    this.loading = false;
    this.error = null;
    this.data = null;
  }

  async fetchData() {
    this.loading = true;
    this.error = null;
    
    try {
      const response = await fetch('https://api.example.com/data');
      if (!response.ok) {
        throw new Error(`HTTP error! status: ${response.status}`);
      }
      this.data = await response.json();
    } catch (error) {
      this.error = error.message;
    } finally {
      this.loading = false;
    }
  }
}

// Usage
const loader = new DataLoader();
loader.fetchData().then(() => {
  if (loader.error) {
    console.error('Failed to load data:', loader.error);
  } else {
    console.log('Data loaded:', loader.data);
  }
});
``` 