# Web Tech

## ****JSON, Storage, DOM, and Event****

### ****JSON****

JSON stands for JavaScript Object Notation, and it is a lightweight data-interchange format. JSON is easy to read and write, making it popular for data transmission and storage. JSON files consist of key-value pairs and arrays, making it similar to a dictionary or a list in Python.

```json
{
  "name": "Mikiyas",
  "age": 30,
  "city": "Adiss Abeba"
}
```

## ****Storage: Session and Local****

Session and Local storage are two ways to store data on the client-side using JavaScript. Both session and local storage store data as key-value pairs.

- **Session Storage:** Stores data temporarily, and the data is deleted when the browser window is closed. Session storage can be useful for storing data that only needs to persist for a single browsing session.
- **Local Storage:** Stores data persistently, even after the browser window is closed. Local storage can be useful for storing data that needs to persist across multiple browsing sessions.

```jsx
// Store data in session storage
sessionStorage.setItem("name", "John");

// Retrieve data from session storage
var name = sessionStorage.getItem("name");

// Store data in local storage
localStorage.setItem("name", "John");

// Retrieve data from local storage
var name = localStorage.getItem("name");
```

## ****DOM - Document Object Model****

The Document Object Model (DOM) is a programming interface for HTML and XML documents. The DOM represents the page so that programs can change the document structure, style, and content. The DOM provides a tree-like structure of elements and their attributes, allowing developers to access and manipulate the HTML and XML document.

```html
<!DOCTYPE html>
<html>
<head>
	<title>DOM Example</title>
</head>
<body>
	<h1 id="title">Hello, World!</h1>
	<p>Click the button to change the title.</p>
	<button onclick="changeTitle()">Change Title</button>
	<script>
		function changeTitle() {
			document.getElementById("title").innerHTML = "New Title";
		}
	</script>
</body>
</html>
```

## ****Event****

An event is an action or occurrence detected by a program, often initiated by the user. In JavaScript, events are used to trigger functions or actions when a user interacts with a webpage. Some common events include clicking a button, typing on a keyboard, or scrolling a webpage.

```html
<!DOCTYPE html>
<html>
<head>
	<title>Event Example</title>
</head>
<body>
	<button onclick="alert('Button clicked!')">Click Me</button>
</body>
</html>
```

## How do we store JSON

**JSON can be stored in various ways, including:**

1. **Text files:** You can save JSON data in a text file with a **`.json`** file extension. This is a common way to store JSON data for use in web applications.
2. **Databases:** JSON data can be stored in databases such as MongoDB, which is a NoSQL database that uses JSON-like documents for data storage.
3. **Server-side storage:** JSON data can be stored on the server using technologies such as Node.js and PHP. This allows you to store and retrieve JSON data from a server-side script.

When storing JSON data, it's important to consider the use case and choose an appropriate storage method that fits your needs.

JavaScript has six primitive data types and one complex data type:

- **Number**: a numeric value, such as 42 or 3.14159.
- **String**: a sequence of characters, such as "Hello, World!" or "123".
- **Boolean**: a logical value, either true or false.
- **Null**: a special value that represents no value or absence of any object value.
- **Undefined**: a special value that represents the absence of a defined value.
- **Symbol**: a unique and immutable data type introduced in ECMAScript 6.
- **Object**: a complex data type that can contain key-value pairs, functions, and other objects.

# **JavaScript Condition**

JavaScript provides conditional statements to execute different actions based on different conditions:

- **if...else**: executes a block of code if a specified condition is true, and another block of code if it is false.
- **switch**: evaluates an expression and executes code associated with the value of the expression.

# **JavaScript Loops**

JavaScript provides loops to execute a block of code repeatedly:

- **for**: executes a block of code a specified number of times.
- **while**: executes a block of code as long as a specified condition is true.
- **do...while**: executes a block of code at least once, and then repeatedly executes the block of code as long as a specified condition is true.
- **for...in**: iterates over the properties of an object.
- **for...of**: iterates over iterable objects such as arrays and strings.

# **JavaScript Object**

JavaScript objects are containers for named values, called properties, and methods. Objects can contain any combination of primitive data types, other objects, and functions.

An object can be created with curly braces {} and properties can be added by assigning values to them:

```jsx
const person = {
  firstName: "John",
  lastName: "Doe",
  age: 30,
  fullName: function() {
    return this.firstName + " " + this.lastName;
  }
};
```

# **JavaScript Function**

JavaScript functions are blocks of code that can be called or invoked to perform a specific task. Functions can take input arguments and return output values.

A function can be defined with the **`function`** keyword:

```jsx
function sayHello(name) {
  console.log("Hello, " + name + "!");
}
```

Functions can also be defined as expressions and assigned to variables:

```jsx
const square = function(x) {
  return x * x;
};
```

# **JavaScript Event**

JavaScript events are actions that occur on a web page, such as a user clicking a button or a page finishing loading. JavaScript can detect these events and execute code in response to them.

Events can be added to HTML elements using event attributes or added dynamically using JavaScript code:

```html
<button onclick="alert('Button clicked!')">Click me</button>
```

```jsx
const button = document.querySelector("button");
button.addEventListener("click", function() {
  alert("Button clicked!");
});
```

# **JavaScript Let vs Var vs Const**

JavaScript provides three ways to declare variables: **`let`**, **`var`**, and **`const`**. Each has different scoping rules and behavior:

- **let**: declares a block-scoped variable that can be reassigned.
- **var**: declares a function-scoped variable that can be reassigned.
- **const**: declares a block-scoped variable that cannot be reassigned.

```html
let x = 5; // block-scoped, can be reassigned
var y = 10; // function-scoped, can be reassigned
const z = 15; // block-scoped, cannot be reassigned
```
