## Notes of Javascript Course

### Syntax

; character after each command
```js
command... ;
command... ;
command... ;
```
// marks a comment till the end of current line  
/* ... */ marks a comment span

```js
// this is a comment
code... ;
/* this is a 
long
comment */
code... ;
```

{ } to create code hierarchies
```js
{ // top-level scope
  { // nested scope
  }
}
```
( ) to prioritize operations
```js
var x = 2;
var y = 3;
var z = (x + y) * 3; // z = 15
```
Case sensitive (keywords & variables)
```js
var x = 5;
X++; // Uncaught ReferenceError: X is not defined
VAR x = 2; // Uncaught SyntaxError: unexpected token: identifier
```
Identifiers (=**variable names** , function names, etc.) should
- not contain spaces.
- begin with a letter, underscore (_) or dollar sign ($).
- only contain letters, numbers, underscores, or dollar signs.
- not be the same as a keyword used by JS

```js
var var = 5; // Uncaught SyntaxError: missing variable name
var 5test = 5; // Uncaught SyntaxError: identifier starts immediately after numeric literal
var using spacebar = 5; // Uncaught SyntaxError: unexpected token: identifier
```
