# Array

- It is a type of data type which can store any types of key charaters in []

  ```js
  cosnt name = ["Ram" , "shyam" , "hari " , ];
  const number = [ "1" , "3" , "4", "9"];
  ```

- crud with array

**C** = ` const boys = [ "Ram", "shyam"];`
**R** =` boys : boys[1]`
**U** = ` boys[1] = "hari"`
**D** = `boys.pop()`

```js
-functions;
const bike = ["hero", "honda", "pulsar"];
const lastIndex = bikes.length - 1;
const lastArrayItem = bikes[lastIndex];
console.log(lastArrayItem); // result = pulsar
```

- functions of array
  `array.push()` = to add new item in array ;
  `array.length` = to find the length in array ;
  `array.pop()` = remove last item in array;
  `array.shift()` = remove first item in array ;
  `array.unshit()` = add a new item in the starting in array ;
  `array.concat()`= to add more item or two items in a single array ;``

- loop-operation

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

for (let i = 0; i < bikes.length; i++) {
  let item = bikes[i];
  console.log(item);
}

//result dominar
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
const description = "This is my first programming language";
const descriptionWords = description.split(" ");
console.log("ds", descriptionWords);
for (let i = 0; i < description.length; i++) {
  let words = descriptionWords[3];
  console.log("position", words);
}
```
