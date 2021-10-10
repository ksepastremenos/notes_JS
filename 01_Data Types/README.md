### Declaring Variables
JS is weak-typed  
More specifically
- You do not specify variable types
- A variable can change data-type via simple assignment  
- functions are treated like a specific data-type
- You do not specify function return-types (ie. integer add(), void print(), etc.)
- There is no such thing as a "delegate"

declaring keywords
- var (obsolete, used to declare variables before JS was used for more complex functions.)
- let (used to declare variables)
- const (used to declare constants)
 
```js
var x = 3;
var x = 2;
let x = 5; //Uncaught SyntaxError: redeclaration of var x
const x = 10; //Uncaught SyntaxError: redeclaration of var x
const z = 10;
z = 15; //Uncaught TypeError: invalid assignment to const 'z'
```

Data types:  
(classes are not covered in this course, so the following are nearly all data types we encountered)

- number // typically a float. JS auto-picks the correct container depending on the number.
```js
let x = 3.5; 
```
- string // text. Indicated with "" (double quotes) or '' (single quotes). There is no difference between the two. 
```js
let y = 'variable containing text'; 
```
- object // JS's main way of pushing around data. Consists of keys and corresponding values.  
```js
let z = { "firstKey": "First Value", "secondKey" : 2, "thirdKey":['an','array','of','strings']}
```
array
undefined
null (typeof == "object")
NaN
