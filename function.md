# JavaScript Functions 🚀

> A simple guide for beginners — if you know basic math, you can learn this!

---

## What is a Function?

A function is a **set of instructions** you write once and use many times.

Think of it like a **vending machine** — you press a button (call the function), it does its job, and gives you something back.

```javascript
function sayHi() {
  console.log("Hi!");
}

sayHi(); // Hi!
sayHi(); // Hi! (use it again!)
```

---

## 3 Ways to Write a Function

### 1. Function Declaration
```javascript
function greet(name) {
  console.log("Hi, " + name + "!");
}

greet("Vivek"); // Hi, Vivek!
```

### 2. Function Expression
```javascript
const greet = function(name) {
  console.log("Hi, " + name + "!");
};

greet("Priya"); // Hi, Priya!
```

### 3. Arrow Function ⚡ (Modern & Short)
```javascript
const greet = (name) => {
  console.log("Hi, " + name + "!");
};

// Even shorter (one line):
const greet = (name) => console.log("Hi, " + name + "!");

greet("Shankar"); // Hi, Shanker!
```

> 💡 All three do the same thing. Arrow functions are the most popular today 😊.

---

## Parameters & Arguments

**Parameter** = the placeholder (in the definition)  
**Argument** = the real value (when you call it)

```javascript
//                👇 parameters
function add(num1, num2) {
  console.log(num1 + num2);
}

//     👇 arguments
add(10, 5); // 15
add(3, 7);  // 10
```

---

## Return — Getting a Value Back

Use `return` when you want the function to **give you a result**.

```javascript
function multiply(a, b) {
  return a * b;
}

const answer = multiply(4, 5);
console.log(answer); // 20
```

> ⚠️ After `return`, the function **stops**. Nothing below it runs.

```javascript
function check(age) {
  if (age >= 18) return "Adult";
  return "Minor"; // only runs if age < 18
}

console.log(check(20)); // Adult
console.log(check(15)); // Minor
```

---

## Default Parameters

Set a **backup value** in case nothing is passed.

```javascript
function welcome(name = "Guest") {
  console.log("Welcome, " + name + "!");
}

welcome("Priya"); // Welcome, Priya!
welcome();         // Welcome, Guest!
```

---

## Scope — Where Can You Use a Variable?

Variables inside a function **stay inside** — they can't be used outside.

```javascript
function myFunc() {
  const secret = "I'm inside!";
  console.log(secret); // ✅ Works
}

myFunc();
console.log(secret); // ❌ ERROR — secret doesn't exist here
```

---

## Common Mistakes ⚠️

```javascript
// ❌ Forgetting () when calling
sayHi;   // Does nothing
sayHi(); // ✅ This works

// ❌ Forgetting return
function square(n) {
  n * n; // result is thrown away!
}

function square(n) {
  return n * n; // ✅ Now it works
}

// ❌ Using a variable outside its scope
function test() {
  const x = 10;
}
console.log(x); // ❌ ERROR
```

---

## Quick Cheatsheet 📋

```javascript
// Declaration
function name(param) { return value; }

// Expression
const name = function(param) { return value; };

// Arrow
const name = (param) => value;

// Default param
function name(param = "default") { }

// Multiple params
function add(a, b) { return a + b; }
```

---

> **Remember:** Write once, use many times. That's the power of functions! 💪😀

<a href="operators.md">previous</a>
<p align=right><a href="controlstatements.md">next</a></p>
