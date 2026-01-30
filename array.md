# Array
A collection of elements under the same name is called as an array.  
Because JavaScript is a dynamic language, arrays don’t have fixed types or lengths.  
An array is like an object whose keys are indexes from 0 to length − 1 and values are the elements.
## 📢 Declaration of arrays
An array is declared using square braces [].  
Array elements need not be of the same type.
```js
// Same data type
let fruits = ["Apple", "Banana", "Cherry"];

// Mixed data types
let mixed = [42, "Hello", true, { name: "Gemini" }];
````
## ⚙️ Operations on array
### 📥 Inserting array elements
|method|description|example|
|-|-|-|
|Direct|simply declare a new element at the end|`fruits[4] = "Blueberry"`|
|push|adds one or more elements to the very end|`fruits.push("Blueberry")`|
|splice|add element anywhere|`fruits.splice(1,0,"Blueberry")`|
|unshift|adds elements to the beginning|`fruits.unshift("Blueberry")`|
### 🗑️ Deleting array elements
|method|description|example|
|-|-|-|
|pop|deletes last element|`fruits.pop()`|
|splice|deletes anywhere|`fruits.splice(1,1)`|
|shift|deletes first element|`fruits.shift()`|
### 🔗 Merging two arrays
concat method is used to add the elements of an array to the end of another array  
`newArray.conacat(oldarray);`  
But using **Spread operator** `[...]` we can:
- Merge two arrays into a new array `let tool = [...frontend, ...backend];`
- Insert new items in the middle `let numbers = [1,...twoTofive,6,7];`
- Combine multiple arrays `let numbers = [...oneTofour, ...fiveToeight, ...nine, 10];`
## 🛠️ Array Functions
|Function name|Description|Example|
|-|-|-|
|length|returns length of the array|`fruits.length`|
|slice|returns part of the array|`fruits.slice(0,3)`|
|indxeOf|returns the index of the element|`fruits.indexOf("Orange")`|
|includes|returns true if array includes th element|`fruits.inlcudes("Apples")`|
|sort|sorts the array|`fruits.sort()`|
|reverse|sorts inreverse order|`fruits.reverse()`|
## 👑 Important methods
Consider `prices = [40,80,230,130,550,95]`
#### 1. map() 🔀
Transforming every array element.
```js
arrayname.map(element => transformation)
// Increase the price of each item by 5%
let newPrices = prices.map(price => price+(price*0.05)); // [42,84,241.5,136.5,572.5,99.25]
````
#### 2. filter() 🔍
Selecting array elements that meet a condition.
```js
arrayname.filter(element => condition)
// Obtain items with price more than 100
let expensivePrices = prices.filter(price => price > 100); // [230,130,550]
````
#### 3. reduce() 🧮
Compress an array into one value
```js
arrayname.reduce((accumulator,element) => expression/function , initialvalue)
// Find the total price
let totalPrice = prices.reduce((sum,price) => sum+price , 0); // 1125
// Find the Maximum price in the prices 
let maxPrice = prices.reduce((large,price) => {return (large<price) ? price : large} , 0); // 550
````
#### 🧵 Chaining of filter, map, reduce
```js
// Find the sum of prices of items pricing more than 100 with 10% of taxes on them
let finalsum = prices
              .map(price => price+(price*0.1)) // Applies 10% tax on each item- [44,88,253,143,605,104.5]
              .filter(price => price > 100) // Selects expensive items- [253,143,605,104.5]
              .reduce((sum,price) => {return sum+price} , 0); // Calculates the sum- 1105.5
````
<br>
<a href="datatype.md">previous</a>
<p align=right><a href="https://github.com/Rohan-Shridhar/javascript">finish</a></p>
