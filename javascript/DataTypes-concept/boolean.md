# Boolean

- [ **true is truthy & false is falsy**]

- It is one of the types of datatypes .
- it can have the following values/data :
  - true
  - false
- Examples
  ```js
  const isLoggedIn = false;
  const isAdmin = true;
  ```

## TRUTHY AND FALSY

- A value is truthy value if it's boolean outcome is true and it's falsy value it's boolean outcome is false.
- Any value can be converted into boolean value using `Boolean()` function.

  ```js
  // in case of string data type
  Boolean(""); // false
  Boolean(" "); // true
  Boolean("sdfghj34567=['?]"); // true
  Boolean("@"); // true

  // in case  number data type
  Boolean(-1); // true
  Boolean(0); // false
  Boolean(1); // true
  Boolean(2); // true

  // in case of boolean data type
  Boolean(true); // true
  Boolean(false); // false

  // other data types
  Boolean(null); // false
  Boolean(undefined); // false
  ```

- Use case :
  - It is needed to whenever and wherever `conditional expression` is needed in the program.
- The output of conditional expression is always have to be either `truthy` or `falsy` in order for the program to continue it's flow of execution of code.

##CRUD

```js
//CREATING A BOOLEAN DATATYPES :
const x = 0;
let sn = 1;

//READ
console.log(x);
console.log(sn);
if (sn > x) {
  console.log("sn is greater than x");
}

//UPDATE
sn = 2;
// console.log(sn);

sn = null;
console.log(sn);
```

## Conditional Statement

```js
if (conditionalExpression) {
}

if (conditionalExperession) {
} else if (conditionalExperession) {
} else if (conditionalExperession) {
} else {
}
```

## Loop

```js
// for (initialization; conditionalExpression; increment/decrement)
for (let i = 0; i < 10; i++) {
  // to do
  console.log(i); //to print 1 to 9
}
```
