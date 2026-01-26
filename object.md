# Object
Object is a real world entity with certain properties.
It is a collection of key-value pairs that specify the object.
```js
let person = {
    name: "Rohan",
    age: 22
};
// Here, person is an object with two properties, name and age which specifies that person.
````
## 📞 Accessing properties
Accessing the object properties is possible in two methods:
- Dot notation
- Bracket notation
```js
console.log(person.name);// Dot notation
console.log(person["age"]);// Bracket notation
````
> [!note]
> If the property to be accessed is determined during run-time, using dot notation won't do the job.
> ```js
> let selection = "name";
> console.log(person.selection);// This doesn't work
> console.log(person[selection]);// This works
> ````

<br>
<a href="datatype.md">previous</a>
<p align=right><a href="array.md">next</a></p>
