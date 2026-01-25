# Datatypes
Datatypes are the type of data a variable can store
- Primitive types
- Reference types

## 🧱 Primitive Types
|Type|description|Example|
|-|-|-|
|Number|Both integers and floating-point numbers (Number literal)|`5`, `5.55`, `Infinity`, `NaN`|
|String|Textual data wrapped in quotes (String literal)|"Hi", 'Hi', \`Hi\`|
|Boolean|Logical values: true or false|`true`, `false`|
|Undefined|A variable that has been declared but not assigned|`undefined`|
|Null|An intentional absence|`null`|

#### Example
```js
let age = 15;
let name = "Rohan";
let isAdult = false;
let Lisence = undefined; // When it is not needed when empty
let favMovie = null; // When it is needed even when empty
````

### 🎭 Dynamic typing
JS is a dynamic language i.e., the type of the variable can change during runtime.
```js
let data = 42;      // data is a Number
data = "Forty-two"; // data is now a String
data = true;        // data is now a Boolean
````

## 🧩 Reference Types
|Type|description|Example|
|-|-|-|
|Object|A collection of properties|`{ name: "John", age: 30 }`|
|Array|A list of values|`[1,2,3]`|
|Function|A block of code||
|Date|object for handling dates and times|`12/10/200`|


<br>
<a href="variables.md">previous</a>
<p align=right><a href="https://github.com/Rohan-Shridhar/javascript">finish</a></p>
