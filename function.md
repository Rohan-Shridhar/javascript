# JavaScript Functions


## ❓ What is a Function?

A function is a set of instructions written once and used many times.  

```javascript
function sayHi() {
  console.log("Hi!");
}

sayHi(); // Hi!
sayHi(); // Hi! (use it again!)
```

---

## 📋 Ways to Write a Function

### 1. Function Declaration  
`function func_name(params) { statements }`  
#### Example
```javascript
function greet(name) {
  console.log("Hi, " + name + "!");
}
````

### 2. Function Expression
`const func_name = function(params) { statements };`  
#### Example
```javascript
const greet = function(name) {
  console.log("Hi, " + name + "!");
};
```

### 3. Arrow Function (Modern & Short)
`const func_name = (params) => { statements };`  
#### Example
```javascript
const greet = (name) => { console.log("Hi, " + name + "!"); };
```
>[!tip]
> 1. `function` keyword 
> 2. `function` and `const` keywords
> 3. `const` keyword

---

## 📥 Parameters & Arguments

**Parameter** = the placeholder in the definition of the function  
**Argument** = the real value passed into the function when you call it  
#### Example
```javascript
//                👇 parameters
function add(num1, num2) {
  console.log(num1 + num2);
}

//     👇 arguments
add(10, 5); // 15
add(x, y);  // x + y
```

---

## ↩️ Return statement

Use `return` when you want the function to **give you a result**.  
#### Example  
```javascript
function multiply(a, b) {
  return a * b;
}

const answer = multiply(4, 5);
console.log(answer); // 20
```

>[!important]
> After `return`, the function **stops**. Nothing below it runs.  
#### Example
```javascript
function check(age) {
  if (age >= 18) return "Adult";
  return "Minor";
  console.log("Thank you!"); // Never executes
}

console.log(check(20)); // Adult
console.log(check(15)); // Minor
```

---

## 🏷️ Default Parameters
Default parameters are set to maintain the function flow incase of no arguemnets being passed in the function call.  
#### Example
```javascript
function welcome(name = "Guest") { // Take value of name as "Guest" whenever no arguements in function call 
  console.log("Welcome, " + name + "!");
}

welcome("Priya"); // Welcome, Priya!
// When no arguements are passed
welcome();         // Welcome, Guest!
```

---

## 🚧 Variable scope

Scope of a variable is the region of the code where it is accessible.  
When variables are declared inside a function, they are called as local variables (function variables) and cannot be accessed outside of the function.  
#### Example
```javascript
function myFunc() {
  const secret = "I'm inside!";
  console.log(secret); // Works
}

myFunc();
console.log(secret); // secret doesn't exist here
```

---

## 🔁 Callbacks
Function callback is used when you want some set of functions to be executed in order without fail.  
#### Example
```js
const sum = (callback, x, y) => {
  let result = 0;  
  setTimeout(() => { result = x + y: }, 3000); // wait for 3s (3000 ms) and then execute { result = x + y; }
  callback(result);
}
const display(result){
  console.log(result);
}

// You want the functions to execute in the order sum() --> display() strictly
// Hence send display as a callback into sum() asking it to execute display() once itself is completely executed.

sum(display, 12, 18); // 18

// No need to write display function separately.

````

<a href="operators.md">previous</a>
<p align=right><a href="controlstatements.md">next</a></p>
