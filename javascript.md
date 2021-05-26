## JAVASCRIPT
* * *

## **HISTORY OF JAVASCRIPT**

- Javascript was created by Brendan Eich in the year 1995.
- The language was written in the time period of 3 weeks.
- The language was developed to use in the browser called Netscape Navigator which was developed by Netscape Communications.
- Javascript and Java are two different languages they do not have any relationship with each other.
- `Javascript` is the only language that can be fully integrated with `html` and `css`.
- The language has its specification called `ECMAScript`.
* * *

## **DATA TYPES IN JAVASCRIPT**
There are mainly two data types present in the language.
1. PRIMITIVE DATA TYPES
2. NON-PRIMITIVE DATA TYPES
* * *

Let's first talk about **primitive data types**. These are the following:
- Number
- String
- Boolean
- Null
- Undefined

**Numbers**: Integers and floating-point numbers.
**String**: Alphanumeric characters.
**Boolean**: true or false
**Null**: Null is means nothing.
**Undefined**: Undefined means the value is not initialized.
* * *
```js
let num = 1; //Number 
let str = 'name';//String
let val = true; //Boolean
let b = null; //Null
let d = undefined; //Undefined

```
* * *
**Non-primitive data types**

- Array
- Object

**Array**: Array is used to store a collection of primitive or non-primitive data types.
**Object**: Object is used to store key-value pair.
* * *
```js
let arr = [1,2,3,4,5]
let obj = {name:'javascript', age:25 }
```
* * *
*In Javascript Variables are like containers which hold something*
* * *
**let var and const**
let var and const are the keywords which are used for the 
declarations.

* * *

| var      | let | const    |
| :---        |    :----:   |          ---: |
| Variable declaration gets hoisted   | Not hoisted      | Not hoisted     |
| Var has functional scope   | let has block/lexical scope        | const has block /lexical scope      |
| It can be redeclared | It cannot redeclare | It cannot redeclare |
| It can be reassigned | It cannot be reassigned | It cannot be reassigned |
| Introduced in ES5      | Introduced in ES6     |Introduced in ES6    |
* * *
**Variable declarations with var**
```js
var name = 'javascript'
var name = 'java'
console.log(name) //output will be java because name can redeclare and reassign also
```
* * *
**Variable declarations with let**
```js
let name = 'javascript'
name = 'python' // 
console.log(name) // python becauese let can reassign its value of the variable
```
* * *

**Variable declarations with const**
```js
const name = 'javascript'
name = 'java' // type error because name cannot be reassign

```
* * *
## **FALSY VALUES**
Falsy values are those value which evaluates as false.
There is a total of five values in javascript which are falsy values.
1. Number - `0`, `NaN`
2. String - ``" "``
3. Undefined - `undefined`
4. NULL - `null`
5. 
* * *

## **OPERATORS IN JAVASCRIPT**
1. Arthmetic Operators  `+` `-` `*` `/` `%` `++` `--` `**` 
2. Logical Operators  `&&(AND)` `||(OR)`
3. Bitwise Operators
4. Ternary Operators 

**CODE**

1. Arthmetic Operators
```js
 console.log(1+2);//simple arthmetic operation
 
```

2. Logical Operators

&&(AND)
```js
console.log(true && true) // true
console.log(false && true ) //false
console.log(true && false) // false
console.log(false && false) //false
```

||(OR)
```js
console.log(true && true) // true
console.log(false && true ) //true
console.log(true && false) // true
console.log(false && false) //false
```
* * *
**typeof**
Javascript has a special keyword for returning the type of variable i.e `typeof`

**Example**
```js
let num = 1;
console.log(typeof(num)) // output: Number
```
* * *

**Hoisting**
- Hoisting is a javascript behaviour to move the variable declaring at the top of the scope.
- Only variable which is declared with the `var` keyword is hoisted.

**Example**
```js
console.log(a)
var a = 'javascript'
//OUTPUT: undefined (because the variable declaration will move to the top and at the top variable is only declare.)

```
* * *

## **FUNCTIONS**
- Functions are nothing but a block of code that is used and design to perform a particular task.
- Functions allow the code to call many times.
- Function can be stored in a variable.
- Function can return another function also.
- Function acts like an object in Javascript.

**Function Declaration with function keyword**
```js
function name(){  // function naming and parameters
    console.log(1+2);  // function body
}
name();// function call
```

**Function stored in variable is called function expression**
```js
let a = function(num){ //function expression
    return num*num; // return statement
}
console.log(a(2)); //OUTPUT: 4

```
* * * 

**Scope in Javascript**
Scope in Javascript represents the availability of variables in code.
In Javascript, there are two types of scope:
1. Global Scope
2. Local Scope

**GLOBAL SCOPE**
Variables which are declared at the top of the code or outside the function are known as global variable.
```js
let global = 1;
function print(){
    console.log(global);
}
print(); //OUTPUT: 1
```
The function can also reassign the value of the global variable.

```js
let global = 1;
function print(){
    global = 2;
    
}
print();
console.log(global) //OUTPUT: 2 
```
**LOCAL SCOPE**
Variables which are declared inside the function is known as local variables and are only accessible to the function.
```js
function local(){
    var x = 'local'
    console.log(x);
}
local(); //OUTPUT: local
```


* * *

## **ARRAY, STRING PROTOTYPE METHODS**
**ARRAY**

| Command | Description |
| --- | --- |
| `push` |push element to the end of the array  |
| `pop` |push element to the end of the array  |
| `unshift` |push element to the end of the array  |
| `shift` |push element to the end of the array  |
| `length` |push element to the end of the array  |
| `concat` |joins two arrays |
| `sort` |sort the array in alphabetical order  |
| `slice` |selects a part of array  |
| `splice` |remove and add a new item in the array  |
| `includes` |checks if the items are available or not  |
| `indexOf` |return the index of the item in the array  |

**STRING**

| Command | Description |
| --- | --- |
| `toLowerCase()` |converts the string in lowercase |
| `toUpperCase()` |converts the string in uppercase  |
| `includes` |checks if the string is present or not  |
| `split` |convert string to array of strings |
| `charAt(index)` |return character of the index   |
| `concat` |joins two strings  |
| `trim` |remove whitespace from the string |
| `slice` |selects a part of array  |
| `splice` |remove and add new item in the array  |
| `includes` |checks if the items is available or not  |



## **BUILT IN FUNCTIONS**


| Command | Description |
| --- | --- |
| `setTimeout` |allows a function to run at a specific time only once |
| `setInterval()` |allows a function to run repeatedly after a specific interval time |
| `parseInt` |converts non-number primtive to a number  |
| `parseFloat` |converts to floating point number |
| `JSON` |Javascript Object Notation  |
