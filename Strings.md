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

## 📞 Accessing characters

Characters of a string are accessed in the same way as array elements are accessed, i.e., is str = "Hello", str[0] is "H".  
However `String.at(index)` function is also used... str.at(-1) will return the last character. 

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
console.log("Javascript".slice(4)); // from the 4th till last index --> "script"
console.log("Javascript".slice(0,4)); // from 0th to 4 -1 = 3rd index --> "Java"
console.log("Javascript".slice(-6)); // last 6 characters --> "script"
````

8. substring - similar to slice but has two non negative integer inputs
```js
console.log("Javascript".substring(0,4)); // "Java"
````

9. replace and replaceAll - used to substitute parts of the string with replacement
```js
console.log("ha ha ha".replace("ha","hi"); // "hi ha ha"
console.log("ha ha ha".replaceAll("ha","hi"); // "hi hi hi"
````

10. split(`delimiter`) - used to convert string into and array
```js
console.log("apples,mangoes,bananas".split(",")); // ["apples","mangoes","bananas"]
````

11. concat() - to attach a string in the end
```js
console.log("Merry".concat(" and ","James"); // Merry and James
````

12. repeat() - used to repeat a string for a number of times
```js
console.log("*".repeat(3)); // "***"
```

13. charAt() - returns the character at the index   
```js
console.log("Javascript".charAt(2)); // "v"
````

14. charCodeAt() - returns the ASCII value of the characte at the index  
```js
console.log("A".charCodeAt(0)); // 65
````

15. padStart() and padEnd() - pad the string to the spefic length by contcatinating the given character to the start or the end  
```js
console.log("5".padStart(3,"0")); // "005"
console.log("5".padEnd(3,"0")); // "500"
````

16. match() - to find substrings using regular expression
```js
console.log("abc123".match(/\d+/)); // "123"
````

17. search() - finds the index of the substring
```js
console.log("hello123".search("/\d/")); // 5
````