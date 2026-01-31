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

#### Illustraction of + operator
```js
[] + 1 --> "" + 1 --> "" + "1" --> "1"
"Hi" + 1 --> "Hi" + "1" --> "Hi1"
true + false --> 1 + 0 --> 1
true + "1" --> "true" + "1" --> "true1"
true + 1 --> 1 + 1 --> 2
null + 1 --> 0 + 1 --> 1
undefined + 1 --> NaN
````
> [!note]
> Other arithmetic operators try to convert all other types into numeric. Ex: "5" - 5 --> 0

## ⚖️Comparison operators

|Operator|Description|Example|Result|
|:-:|:-:|:-:|:-:|
|==|equal to|true == 1|true|
|===|exactly equal to|true === 1|false|
|!=|not equal to|true != 1|false|
|<|Less than|1 < 3|true|
|>|Greater than|4 > 5|false|
|<=|Less than or equal to|1 <= 1|true|
|>=|Greater than or equal to|10 >= 20|false|

<br>
<a href="array.md">previous</a>
<p align=right><a href="https://github.com/Rohan-Shridhar/javascript">finish</a></p>
