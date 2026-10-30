# JavaScript Math Object

`Math` is a built-in JavaScript object that provides a collection of properties and methods related to mathematical operations.

**Examples:**
```js
console.log(Math.PI) // 3.141592653589793
console.log(Math.E)  // 2.718281828459045
```

## 📐 Math Methods

### 1. round() method

The `Math.round()` method rounds a decimal number to the nearest integer.

```js
console.log(Math.round(3.4)) // 3
console.log(Math.round(3.7)) // 4
```

### 2. floor() method

The `Math.floor()` method rounds a number down to the greatest integer less than or equal to the given number.

```js
console.log(Math.floor(3.9))  // 3
console.log(Math.floor(-3.2)) // -4
```

### 3. ceil() method

The `Math.ceil()` method rounds a number up to the smallest integer greater than or equal to the given number.

```js
console.log(Math.ceil(3.22)) // 4
console.log(Math.ceil(3.8))  // 4
```

### 4. trunc() method

The `Math.trunc()` method removes all decimal places and keeps only the integer part of the number.

```js
console.log(Math.trunc(3.88))  // 3
console.log(Math.trunc(-3.88)) // -3
```

### 5. abs() method

The `Math.abs()` method returns the absolute (non-negative) value of a number. It is similar to the modulus operation.

```js
console.log(Math.abs(-2.03)) // 2.03
console.log(Math.abs(5))     // 5
```

### 6. pow() and sqrt() methods

- `Math.pow()` returns a number raised to a specified power.
- `Math.sqrt()` returns the square root of a number.

```js
console.log(Math.pow(2, 3)) // 8

console.log(Math.sqrt(81)) // 9
```

### 7. log() method

The `Math.log()` method returns the natural logarithm of a number, that is, the logarithm to base **e (approximately 2.718)**.

```js
console.log(Math.log(10)) // 2.302585...
```

### 8. Trigonometric functions

JavaScript provides trigonometric functions through the `Math` object.

```js
console.log(Math.sin(0)) // 0

console.log(Math.cos(0)) // 1

console.log(Math.tan(0)) // 0
```

>**Note**  
>
> Trigonometric functions accept angles in radians, not degrees.

### 9. sign() method

The `Math.sign()` method returns:
- `-1` for negative numbers.
- `1` for positive numbers.
- `0` for zero.

```js
console.log(Math.sign(-9)) // -1
console.log(Math.sign(0))  // 0
console.log(Math.sign(9))  // 1
```

---

> **Note**
>
> You can assign numbers to variables and pass those variables to Math methods instead of passing numbers directly.

```js
let num = 3.8;

console.log(Math.round(num)) // 4
console.log(Math.floor(num)) // 3
```

## Quick Revision Table

| Method | Purpose |
|---|---|
| `Math.round()` | Rounds to nearest integer |
| `Math.floor()` | Rounds down |
| `Math.ceil()` | Rounds up |
| `Math.trunc()` | Removes decimal part |
| `Math.abs()` | Returns absolute value |
| `Math.pow()` | Calculates power |
| `Math.sqrt()` | Calculates square root |
| `Math.log()` | Returns natural logarithm |
| `Math.sin()` | Calculates sine |
| `Math.cos()` | Calculates cosine |
| `Math.tan()` | Calculates tangent |
| `Math.sign()` | Returns sign of a number |
