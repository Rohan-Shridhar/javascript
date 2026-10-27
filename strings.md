# Strings
 A string is a sequence of characters used to store text data.

```js
let name = "Rohan";
let city = "Bangalore";
````
Strings can be enclosed in "", '' or ``

## 👶 Creating strings

For creating a string, `new String("Hello")` is rarely used, primitive and simple way is used to define and declare strings.

```js
let message = "Hi";
````
### 🔒 String Immutability

Strings are immutable, meaning their characters cannot be changed directly after creation.

```js
let str = "Hello";
str[0] = "Y";

console.log(str); // "Hello"
```
String methods return new strings instead of modifying the original string.

## 📞 Accessing Characters

Characters can be accessed using square bracket notation or the `at()` method. Indexing starts from `0`.

```js
let str = "Hello";

console.log(str[0]);   // "H"
console.log(str.at(0));  // "H"
console.log(str.at(-1)); // "o" (last character)
```
> [!note]
> Negative indices work with at(), but not with square bracket notation.

## String properties

length property
```js
let str = "javascript is amazing";
console.log(str.length); // returns the length of the string including blank spaces.
````

## ⚙️ String methods

1. ToUppercase() - to convert all characters into uppercase alphabets
```js
console.log("hi".toUpperCase()); // "HI"
````

2. toLowerCase() - to convert all characters into lowercase alphabets
```js
console.log("HI".toLowerCase()); // "hi"
````

3. trim methods
```js
console.log(" hi ".trim()); // "hi"
console.log(" hi ".trimStart()); // "hi "
console.log(" hi ".trimEnd()); // " hi"
````

4. includes() - returns true if the input string is a substring of the string
```js
console.log("Javascript".includes("Java")); // true
console.log("Javascript".includes("Python")); // fasle
````

5. startsWitn and endsWith methods
```js
console.log("Javascript".startsWith("Java")); // true
console.log("Javascript".startsWith("Python")); // fasle

console.log("Javascript".endsWith("script")); // true
console.log("Javascript".endsWith("lang")); // fasle
````

6. indexOf() and lastIndexOf() - return the first or last index of the substringin the string, or else reutrn -1 if not present
```js
console.log("java".indexOf("a")); // 1
console.log("java".lastIndexof("a")); // 3
````

7. slice() - used to extract part of the string
```js
console.log("Javascript".slice(4)); // from the 4th till last index --> "script"
console.log("Javascript".slice(0,4)); // from 0th to 4 -1 = 3rd index --> "Java"
console.log("Javascript".slice(-6)); // last 6 characters --> "script"
````

8. `substring()` - extracts a part of a string using start and end indices. The end index is excluded.

```js
console.log("Javascript".substring(0, 4)); // "Java"
console.log("Javascript".substring(4));    // "script"
```

> [!note]
> Unlike slice(), substring() treats negative indices as 0 and swaps the arguments if the start index is greater than the end index.

// 9. replace() and replaceAll() - used to substitute parts of the string with replacement
```js
console.log("ha ha ha".replace("ha", "hi"));    // "hi ha ha"
console.log("ha ha ha".replaceAll("ha", "hi")); // "hi hi hi"
```

10. split(`delimiter`) - used to convert string into and array
```js
console.log("apples,mangoes,bananas".split(",")); // ["apples","mangoes","bananas"]
````

// 11. concat() - to attach a string in the end
```js
console.log("Merry".concat(" and ", "James")); // "Merry and James"
```

12. repeat() - used to repeat a string for a number of times
```js
console.log("*".repeat(3)); // "***"
```

13. charAt() - returns the character at the index   
```js
console.log("Javascript".charAt(2)); // "v"
````

// 14. charCodeAt()  - returns the ASCII value of the characte at the index  
```js
console.log("A".charCodeAt(0)); // 65
```

15. padStart() and padEnd() - pad the string to the spefic length by contcatinating the given character to the start or the end  
```js
console.log("5".padStart(3,"0")); // "005"
console.log("5".padEnd(3,"0")); // "500"
````

16. match() - to find substrings using regular expression
```js
console.log("abc123".match(/\d+/)); // "123"
````

// 17. search() - finds the index of the substring
```js
console.log("hello123".search(/\d/)); // 5
```
> [!note]
> `String("Hello")` returns a primitive string, whereas `new String("Hello")` creates a String object. Prefer primitive strings.
>  ```js
> console.log(typeof String("Hello"));     // "string"
> console.log(typeof new String("Hello")); // "object"
> ```
<br>
<a href="Math_object.md">previous</a>
<p align=right><a href="array.md">next</a></p>
