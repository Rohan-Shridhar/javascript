# Variables
Variables are the containers for storing values or expressions
#### Example
```js
section = "3U"
console.log(section)
````
## ⚖️ Rules for js variables
- Case sensitive
- Must start with an an alphabet or underscore
- Cannot start with a number
- Cannot use reserved words as variables
#### Here are few examples:
- score ✅
- _id ✅
- 01 🚫
- await 🚫
<br>

## 📢 Declaration of varaibles
There are three methods of declaring a variable in js
- let keyword
- const keyword
- var keyword

|Keyword|Access|Assignment|Initialise|
|-|-|-|-|
|let|{...}|Reassignable|Optional|
|const|{...}|Final|Required|
|var|function|Reassignable|Optional|

#### Reassignment
```js
let count = 0
count = 1 //This works

const count = 0
count = 1 //This doesn't work

var count = 0
count = 1 //This works
````

#### Accessibility
```js
{
  let blockVariable = "I am hidden";
  var functionVariable = "I am visible";
}

console.log(blockVariable);    //This doesn't work
console.log(functionVariable); //This works
````

#### Note
- If you assign values to variables that have not yet been declared, the variables will automatically be declared.
- "var" has some confusing behaviors regarding scope and hoisting, so modern developers generally avoid it in favor of let and const.
