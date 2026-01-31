# Operators
Operatoes are symbols used to execute certian operations represented by it.
## 🧮 Arithmetic operators
Consider `y = 5` 
|Operator|Example|Result|Description|
|:---:|:---:|:---:|:---:|
|+|x = y + 2|7|Addition|
|-|x = y - 2|3|Subtraction|
|*|x = y * 2|10|Multiplication|
|/|x = y / 2|2.5|Division|
|%|x = y % 2|1|Modulo|
|++|x = ++y|6|Increement|
|--|x = --y|4|Decreement|
## 🟰 Assignment operators
Consider `x = 10 y = 5`
|Operator|Example|Result|Description|
|:---:|:---:|:---:|:---:|
|=|x = y|5||
|+=|x += y|15|x=x+y|
|-=|x -= y|5|x=x-y|
|*=|x *= y|50|x=x*y |
|/=|x /= y|2|x=x/y|
|%=|x %= y|0|x=x%y|

### ➕ operator logic
The + operator can also be used to add string variables or text values together.  
```js
txt1="What a very "; 
txt2="nice day"; 
txt3=txt1+txt2; // What a very nice day
````

With mixed data types, the + operator causes JavaScript to run through a set sequence of **type conversions**  
> If Object/Array is present -> Convert into primitive\
>     If not\
> If String is present -> Convert into String and concatenate\
> IF not\
> Convert into Numeric type and add\
> If not possible to even convert into number\
> return NaN
