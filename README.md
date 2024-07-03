# Document Object Model (DOM) - README

## Introduction
The Document Object Model (DOM) is a programming interface for web documents. It represents the structure of a document as a tree of objects, making it possible for programming languages like JavaScript to manipulate the content, structure, and style of web pages dynamically. The DOM provides a way to access and change the content of HTML and XML documents programmatically.

## Major Methods and Properties

### Selecting Elements
- **`document.getElementById(id)`**: Selects an element by its ID.
  ```javascript
  var element = document.getElementById('myId');
- **`document.getElementsByClassName(className)`**: Selects all elements with a specified class.
  ```javascript
  var elements = document.getElementsByClassName('myClass');
- **`document.getElementsByTagName(tagName)`**: Selects all elements with a specified tag name.
  ```javascript
  var elements = document.getElementsByTagName('div');
- **`document.getElementsByTagName(tagName)`**: Selects all elements with a specified tag name.
  ```javascript
  var elements = document.getElementsByTagName('div');
- **`document.querySelector(selector)`**: Selects the first element that matches a CSS selector.
  ```javascript
  var element = document.querySelector('.myClass');
- **`document.querySelectorAll(selector)`**: Selects all elements that match a CSS selector.
  ```javascript
  var elements = document.querySelectorAll('.myClass');

### Manipulating elements
- **`element.innerHTML`**: Gets or sets the HTML content inside an element.
  ```javascript
  element.innerHTML = '<p>New Content</p>';
- **`element.textContent`**: Gets or sets the text content inside an element.
  ```javascript
  element.textContent = 'New Text';
- **`element.setAttribute(name, value)`**: Sets the value of an attribute on the specified element.
  ```javascript
  element.setAttribute('class', 'newClass');
- **`element.getAttribute(name)`**: Gets the value of an attribute on the specified element.
  ```javascript
  var className = element.getAttribute('class');
- **`element.classList.add(className)`**: Adds a class to the element.
  ```javascript
  element.classList.add('newClass');
- **`element.classList.remove(className)`**: Removes a class from the element.
  ```javascript
  element.classList.remove('oldClass');
- **`element.classList.toggle(className)`**: Toggles a class on the element.
  ```javascript
  element.classList.toggle('active');

### Creating or removing elements
- **`document.createElement(tagName)`**: Creates a new element.
  ```javascript
  var newDiv = document.createElement('div');
- **`element.appendChild(child)`**: Appends a child element to the specified element.
  ```javascript
  var parent = document.getElementById('parent');
  parent.appendChild(newDiv);
- **`element.removeChild(child)`**: Removes a child element from the specified element.
  ```javascript
  parent.removeChild(newDiv);

### Event Handling
- **`element.addEventListener(event, function)`**: Adds an event listener to the element.
  ```javascript
  element.addEventListener('click', function() {
    alert('Element clicked!');
  });
- **`element.removeEventListener(event, function)`**: Removes an event listener from the element.
  ```javascript
  function handleClick() {
    alert('Element clicked!');
  }
  element.removeEventListener('click', handleClick);
