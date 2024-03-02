# Array

- [ **All types array store truthy value** ]
- It is a type of data type which can store any types of key charaters in [ ]

- **crud with array**

**C** = ` const boys = [ "Ram", "shyam"];` //create
**R** =` boys : boys[1]` //read
**U** = ` boys[1] = "hari"` //update
**D** = `boys.pop()` //delete last item
**D** = `boys.shift()` //delete first item

- **functions**

```js
const bike = ["hero", "honda", "pulsar"];
const lastIndex = bikes.length - 1; //get the item at last index
const lastArrayItem = bikes[lastIndex];
console.log(lastArrayItem); // result = pulsar
```

```js
- functions of array
  `array.push()` = to add new item in the last of an array ;
  `array.length` = to find the length in array ;
  `array.pop()` = remove last item in array;
  `array.shift()` = remove first item in array ;
  `array.unshit()` = add a new item in the starting in array ;
  `array.concat()`= to add more item or two items in a single array ;``
```

- **CURD OPERATION ON AN ARRAY**

```js
//#CREATING

//creating empty variable adding items into array
var fruits = null;
fruits = ["apple", "banana", "orange", "mango"];

//READING

//printing item of an array
console.log("print fruits =", fruits);

//printing the length of an array
console.log("print fruits length =", fruits.length);

//printing 3rd item in the array
console.log("print 3rd of fruits =", fruits[2]);

//#UPDATE

//remove first item form the array [ shift & unshift method]
console.log("remove first item from fruits array = ", fruits.shift());
console.log("after remove first item from fruits array = ", fruits);
console.log(fruits.unshift("apple"));
console.log(fruits);
console.log(fruits.unshift("grapes"));
console.log(fruits);

//replacing second item of an array [converting array to string and replacing by replace.string method]

var tostring = fruits.toString();
console.log(tostring); // Result : apple,banana,orange,mango
var nString = tostring.replace("apple", "litchi");
console.log(nString); //Result : litchi,banana,orange,mango
var fruits = nString.split(",");
console.log(fruits); //Result : [ 'litchi', 'banana', 'orange', 'mango' ]

//adding a new item called cherry in the last item of an array
console.log(fruits.push("cherry"));
console.log(fruits); //Result : [ 'litchi', 'banana', 'orange', 'mango' ,"cherry"]

//DELETE

//removing first item of an aray
console.log(fruits.shift());
console.log(fruits); //Result : [  'banana', 'orange', 'mango' ,"cherry"]

//removing last item from an array
console.log(fruits.pop());
console.log(fruits); //Result : [  'banana', 'orange', 'mango' ,]

//removing 2nd item of an array
fruits = ["apple", "banana", "orange", "mango"];
var toNewString = fruits.toString();
var nNstring = toNewString.replace("banana", "");
console.log(nNstring);
var fruits = nNstring.split(",");
console.log(fruits); //Result : [ 'apple', '', 'orange', 'mango' ]
fruits.push("banana");
console.log(fruits); //Result : [ 'apple', '', 'orange', 'mango', 'banana' ]

//Check if "Banana" is in the array. If it is, remove it.

var fruits = ["apple", "ball", "banana", "gauva"];

var newFruits = [];
for (let i = 0; i < fruits.length; i++) {
  var item = fruits[i];
  if (item !== "banana") {
    newFruits.push(item);
  }
}
console.log(newFruits); //Result[ 'apple', 'ball', 'gauva' ]
```

```js
var fruits = ["apple", "ball", "banana", "gauva"];
let vegetables = ["patato", "cauli", "tamato"];
let vegetablesAndFruits = fruits.concat(vegetables);
console.log(vegetablesAndFruits); //Result :
//[
//'apple',  'ball',
//'banana', 'gauva',
//'patato', 'cauli',
//'tamato'
//]

//loop on array to ascess item
let v = [];
for (let i = 0; i < vegetables.length; i++) {
  let item = vegetables[i];
  v.push(item);
}
console.log(v);

//Result :
//[
//'apple',  'ball',
//'banana', 'gauva',
//'patato', 'cauli',
//'tamato'
//]
```

- **Loop-operation**

- print items of bikes

```js
const bikes = [
  "dominar",
  "ns",
  "pulsar",
  "discover",
  "pulsar220",
  "nk",
  "nk200",
  "pulsar",
  "dominar",
  "pulsar",
  "ns",
];

for (let i = 0; i < bikes.length - 1; i++) {
  let item = bikes[i];
  console.log(item);
}

//result:

// dominar
// ns
// pulsar
// discover
// pulsar220
// nk
// nk200
// pulsar
// dominar
// pulsar
// ns
```

- convert string to array and operate in loop

```js
//print the each word of the string though loop

const description = "This is my first programming language";
const descriptionWords = description.split(" "); //[ 'This', 'is', 'my', 'first', 'programming', 'language' ]
console.log("ds", descriptionWords);
for (let i = 0; i < description.length; i++) {
  let words = descriptionWords[3];
  console.log("position", words);
}

//This
//is
//my
//first
//programming
//language
```
