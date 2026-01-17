# Variables
Variables are the containers for storing values or expressions
## ⚖️ Rules for js variables
- They are case sensitive
- Must start with a letter or an underscore
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

|Keyword|Access|Assignment|
|-|-|-|
|let|{...}|Reassignable|
|const|{...}|Final|
|var|function|Reassignable|

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
- "var" has some confusing behaviors regarding scope, so modern developers generally avoid it in favor of let and const.
