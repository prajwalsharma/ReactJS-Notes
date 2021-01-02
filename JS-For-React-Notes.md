# 1. var & let

1. **var** - to create value with global scope (old)
2. **let** - to create a variable (new) (ES6)
3. **const** - to create a constant value. It will throw error if you reassign again. (ES6)



# 2. Arrow Functions

Arrow functions are shorter way to write functions in JS.

```javascript
// Normal Function
function PrintName(name){
    console.log(name);
}

// Call normal function
PrintName("Prajwal");	// Prajwal

// Arrow Function
const printName = (name) => {
    console.log(name);
}

// Call Arrow Function
printName("Prajwal");	// Prajwal
```



# 3. Import & Export

1. **Import** - We can import content from other JS files.

2. **Export** - We can export content from current JS file, so that other JS files can Import this.

   a. **export default**

   ​	It means we'll be exporting only one selected content by default.

   b. **export (without default)**

   ​	It means we'll be exporting only a particular module for current JS file.

   ```javascript
   // Default Export
   
   import person from './person.js'
   import prs from '.person.js'
   
   // Normal Export
   import {something} from './utility.js'
   import {something as smth} from './utility.js'
   import * as bundled from './utility.js'
   ```



# 4. Classes

Just like classes in C# & Java

```javascript
class Human{
  constructor(){
    console.log('Human Constructor is called');
    this.gender = 'male';
  }

  printGender(){
    console.log(this.gender);
  }
}

class Person extends Human{

  constructor(){
    super();
    console.log('Person Constructor is called');
    this.name = "Prajwal";
    this.gender = 'female';
  }

  printName(){
    console.log(this.name);
  }
}

const person = new Person();
console.log(person.name);
console.log(person.printGender());
```



# 5. Classes, Properties & Methods

1. **Properties** are like variables attached to classes/objects.

2. **Methods** are like functions attached to classes/objects.

   ```javascript
   // Properties
   // ES6 way
   constructor(){
       this.gender = 'male';
   }
   
   // ES7 way
   gender = 'male'
   
   
   // Methods
   // ES6 way
   myMethod(){}
   
   // ES7 way
   myMethod = () => {}
   ```

   ```javascript
   // ES 7 way
   class Human{
     gender = 'male';
   
     printGender = () => {console.log(this.gender);}
   }
   
   class Person extends Human{
     name = 'Max';
     gender = 'female';
   
     printName = () => {console.log(this.name);}
   }
   
   const person = new Person();
   person.printGender();
   person.printName();
   ```

    

# 6. Spread & Rest operator (...)

1. **Spread**

   This operator is used to split up array elements or object properties.

   ```javascript
   // Copy elements from old to new array
   const newArray = [...oldArray];
   
   // Copy elements from old to new object
   const newObject = {...oldObject};
   ```

2. **Rest**

   This is used to merge a list of function arguments into an array.

   ```javascript
   function myFunction(...args){
       return args.Sort();
   }
   ```

   

# 7. Destructuring

Using this, we can easily extract elements or object properties and store them in variables.

```javascript
// Array destructuring
const numbers = [1,2,3,4];
[num1, num2] = numbers;
console.log(num1, num2);	// 1 2

// Object Destructuring
{name} = {name: 'Prajwal', age: 27};
console.log(name);	// Prajwal
console.log(age); // undefined
console.log(object.age);	// 27
```



# 8. Array Functions

```javascript
// Perform an action on each element on the array
const numbers = [1,2,3,4];

const abc = numbers.map((num) => {
  return num * 2
});

console.log(abc)
```

