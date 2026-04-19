# Math Object
Math is a built-in javascript object that provides a collection of properties and  methods related to mathematics.  
Example: Math.PI, Math.E

## 📐 Math methods
- ### round() method is used to round the decimal to nearest integer
```js
console.log(Math.round(3.4)) // 3
````
- ### floor() method is used to reduce the decimal to the highest integer lesser than itself
```js
console.log(Math.floor(3.9)) // 3
````
- ### ceil() method is used to increase the decimal to the lowest integer greater than itself
```js
console.log(Math.ceil(3.22)) // 4
````
- ### trunc() method is used to ignore all the decimal places and keep just the integer
```js
console.log(Math.trunc(3.88)) // 3
````
- ### abs() methods to convert negative to positve number (mod function)
```js
console.log(Math.abs(-2.03)) // 2.03
````
- ### pow() and sqrt() methods
```js
console.log(Math.pow(2,3)) // 8

console.log(Math.sqrt(81)) // 9
````
- ### log() methods returns the logarithm of the number to the base e (= 2.71)
```js
console.log(Math.log(10)) // 2.3
````
- ### Trignometric functions as Math object methods
```js
console.log(Math.sin(0)) // 0

console.log(Math.cos(0)) // 1

console.log(Math.tan(0)) // 0
````
- ### sign() method return -1 for negative, 1 for positive and 0 for zero
```js
console.log(Math.sign(-9)) // -1
console.log(Math.sign(0)) // 0
console.log(Math.sign(9)) // 1
````
>[!note]
>You can assign numbers to variables and pass variables to methods instead.
