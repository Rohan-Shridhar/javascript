# 🤔 Why is conditional and looping statements important??
- **Conditionals enable decision-making** — programs can choose different actions based on input or situations (e.g., if user is logged in, show dashboard).

- **Loops enable repetition** — they allow running the same block of code multiple times without rewriting it (e.g., processing lists, displaying items).

- **Together they create real logic** — combining loops with conditionals lets programs handle complex tasks efficiently (e.g., iterate through data and apply conditions).
# Conditional Statements 🔀
Very often when you write code, you want to perform different actions for different decisions. You can 
use conditional statements in your code to do this. 
## 1️⃣ If statement
If you want to execute some code only if a specified condition is true.  
```js
// Syntax
if (condition) 
{ 
code to be executed if condition is true 
} 

// Example
if (time<10)  
{ 
document.write("<b>Good morning</b>"); 
} 
````
## 2️⃣ If....else statement
If you want to execute some code if a condition is true and another code if the condition is not true, 
```js
// Syntax
if (condition) 
{ 
code to be executed if condition is true 
} 
else 
{ 
code to be executed if condition is not true 
} 

// Example
if (time < 10)  
{ 
document.write("Good morning!"); 
} 
else 
{ 
document.write("Good day!"); 
} 
````
## 3️⃣ Switch statement
If you want to select one of many blocks of code to be executed.
```js
// Syntax
switch(expression) 
{ 
case label-1: 
  execute code block 1 
  break;     
case label-2: 
  execute code block 2 
  break; 
default: 
  code to be executed if expression is 
  different from label-1 and label-2 
} 

// Example
switch (theDay) 
{ 
case 5: 
  document.write("Finally Friday"); 
  break; 
case 6: 
  document.write("Super Saturday"); 
  break; 
case 0: 
  document.write("Sleepy Sunday");
  break; 
default: 
document.write("I'm looking forward to this weekend!"); 
} 
````
# Looping Statements 🔁
Very often when you write code, you want the same block of code to run over and over again in a row. 
Instead of adding several almost equal lines in a script we can use loops to perform a task like this.   
## 1️⃣ for loop
The for loop is used when you know in advance how many times the script should run.  
```js
// Syntax
for (initialisation ; condition ; increment/decrement )  
{ 
code to be executed 
}

// Example
for(var i = 1; i <= 10; i++)
{
  console.log(i);
}
````
## 2️⃣ while loop
The while loop is used when you want the loop to execute and continue executing while the specified 
condition is true.  
```js
// Syntax
Initialisation
while (condition) 
{ 
    code to be executed
    Update variable 
}

// Example
var i=0; 
while (i <= 10) 
{ 
  console.log(i);
  i=i+1; 
} 
````
## 3️⃣ do....while loop
This loop will always be executed at least once, even if the condition is false, because the code is executed before the condition is 
tested.  
```js
// Syntax
Initialisation
do 
{ 
    code to be executed
    Update variable
} 
while (condition);

// Example
var i=0; 
do  
{ 
    console.log(i);
    i=i+1; 
} 
while (i <= 10); 
````


<a href="function.md">previous</a>
<p align=right><a href="https://github.com/Rohan-Shridhar/javascript">finish</a></p>
