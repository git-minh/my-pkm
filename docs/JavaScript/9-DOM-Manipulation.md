---
sidebar_position: 9
---

### 9. **DOM Manipulation**
- **Selecting Elements:** `getElementById()`, `querySelector()`, `querySelectorAll()`
- **Modifying Elements:** `innerHTML`, `textContent`, `setAttribute()`
- **Event Handling:** `addEventListener()`

#### **Selecting Elements**

```javascript
// By ID
const element = document.getElementById('myId');

// By class name
const elements = document.getElementsByClassName('myClass');

// By tag name
const divs = document.getElementsByTagName('div');

// Using querySelector
const firstElement = document.querySelector('.myClass');

// Using querySelectorAll
const allElements = document.querySelectorAll('.myClass');
```

#### **Modifying Elements**

1. **Changing Content**
```javascript
// Using innerHTML
element.innerHTML = '<span>New content</span>';

// Using textContent
element.textContent = 'New text content';

// Using innerText
element.innerText = 'New text';
```

2. **Modifying Attributes**
```javascript
// Setting attributes
element.setAttribute('class', 'newClass');
element.setAttribute('data-id', '123');

// Getting attributes
const className = element.getAttribute('class');

// Removing attributes
element.removeAttribute('data-id');
```

3. **Modifying Styles**
```javascript
// Using style property
element.style.backgroundColor = 'red';
element.style.fontSize = '16px';

// Using classList
element.classList.add('newClass');
element.classList.remove('oldClass');
element.classList.toggle('active');
element.classList.contains('active');
```

#### **Creating and Removing Elements**

1. **Creating Elements**
```javascript
// Create new element
const newDiv = document.createElement('div');
newDiv.textContent = 'New Element';

// Add to document
document.body.appendChild(newDiv);

// Insert before another element
const referenceElement = document.getElementById('reference');
document.body.insertBefore(newDiv, referenceElement);
```

2. **Removing Elements**
```javascript
// Remove element
element.remove();

// Remove child element
parent.removeChild(child);
```

#### **Event Handling**

1. **Adding Event Listeners**
```javascript
// Click event
element.addEventListener('click', function(event) {
  console.log('Element clicked!');
});

// With event object
element.addEventListener('click', function(event) {
  console.log(event.target);
  console.log(event.type);
});

// Mouse events
element.addEventListener('mouseover', function() {
  console.log('Mouse over!');
});

element.addEventListener('mouseout', function() {
  console.log('Mouse out!');
});
```

2. **Removing Event Listeners**
```javascript
function handleClick() {
  console.log('Clicked!');
}

element.addEventListener('click', handleClick);
element.removeEventListener('click', handleClick);
```

#### **Practical Examples**

1. **Form Handling**
```javascript
const form = document.getElementById('myForm');
const input = document.getElementById('myInput');

form.addEventListener('submit', function(event) {
  event.preventDefault();
  console.log('Form submitted:', input.value);
});
```

2. **Dynamic List**
```javascript
const list = document.getElementById('myList');
const addButton = document.getElementById('addButton');

addButton.addEventListener('click', function() {
  const newItem = document.createElement('li');
  newItem.textContent = 'New Item';
  list.appendChild(newItem);
});
```

3. **Toggle Menu**
```javascript
const menuButton = document.getElementById('menuButton');
const menu = document.getElementById('menu');

menuButton.addEventListener('click', function() {
  menu.classList.toggle('active');
});
```

4. **Image Gallery**
```javascript
const images = document.querySelectorAll('.gallery-image');
const mainImage = document.getElementById('mainImage');

images.forEach(image => {
  image.addEventListener('click', function() {
    mainImage.src = this.src;
    images.forEach(img => img.classList.remove('active'));
    this.classList.add('active');
  });
});
```

5. **Form Validation**
```javascript
const form = document.getElementById('registrationForm');
const username = document.getElementById('username');
const email = document.getElementById('email');

form.addEventListener('submit', function(event) {
  event.preventDefault();
  
  if (username.value.length < 3) {
    showError(username, 'Username must be at least 3 characters');
    return;
  }
  
  if (!isValidEmail(email.value)) {
    showError(email, 'Please enter a valid email');
    return;
  }
  
  // Submit form if validation passes
  this.submit();
});

function showError(element, message) {
  const errorDiv = element.nextElementSibling;
  errorDiv.textContent = message;
  errorDiv.classList.add('error');
}

function isValidEmail(email) {
  return /^[^\s@]+@[^\s@]+\.[^\s@]+$/.test(email);
}
``` 