##DATA-TRAVERSAL

- **The process of visiting content of datatypes atleast once is Data-Traversal.**

  -for example :

  1. string = visiting a string by each character or by word.
  2. array = visiting item of an array
  3. object = visiting only key ,
     visiting only values, visiting key and values together

## String

- array by indexing

- **1. print the all letters of myName**

```js
// expected output =
//a
// f
// r
// o
// j

// s
// i
// d
// d
// i
// k
// i
```

```js
const myName = "afroj siddiki";
const splitName = myName.split("");
// for (let i = 0; i < splitName.length; i++) {
//   const element = splitName[i];
//   console.log(element);
// }

splitName.forEach(function (item, i) {
  console.log(item);
});

//output =
//a
//f
//r
//o
//j

//s
//i
//d
//d
//i
//k
//i
```

// char

- **2. print the all letters of fullName**

```js
// expected output =
//a
// f
// r
// o
// j

// s
// i
// d
// d
// i
// k
// i
```

```js
const fullName = "afroj siddiki";
for (let i = 0; i < fullName.length; i++) {
  item = fullName.charAt(i);
  console.log(item);
}

//output =
//a
//f
//r
//o
//j

//s
//i
//d
//d
//i
//k
//i
```

## Array

- array of string
- **1. print the all names**

```js
// expected output =
//firoj;
//saharoj;
//afroj;
//shoaib;
//jayad;
```

```js
const names = ["firoj", "saharoj", "afroj", "shoaib", "jayad"];

for (let i = 0; i < names.length; i++) {
  const element = names[i];
  console.log(element);
}

//output =
//firoj;
//saharoj;
//afroj;
//shoaib;
//jayad;
```

```js
const myName = "afroj siddiki";
const splitName = myName.split("");
for (let i = 0; i < splitName.length; i++) {
  const element = splitName[i];
  console.log(element);
}
//output =
//a
//f
//r
//o
//j

//s
//i
//d
//d
//i
//k
//i
```

// array of number

- **print the all the numbers from myNum**

```js
//output =
//1
//2
//3
//4
//5
//6
//7
//8
//9
//10
```

```js
const myNum = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
for (let index = 0; index < myNum.length; index++) {
  const element = myNum[index];
  console.log(element);
}

//output =
//1
//2
//3
//4
//5
//6
//7
//8
//9
//10
```

// array of object

- **3. Print the array of object**

```js
// Expected Output={ brand: 'Bajaj', model: 'ns200', cc: 200 }
// { brand: 'honda', model: 'cbz', cc: 150 }
```

```js
const bikes = [
  {
    brand: "Bajaj",
    model: "ns200",
    cc: 200,
  },
  {
    brand: "honda",
    model: "cbz",
    cc: 150,
  },
];
for (let index = 0; index < bikes.length; index++) {
  const element = bikes[index];
  console.log(element);
}
//output={ brand: 'Bajaj', model: 'ns200', cc: 200 }
// { brand: 'honda', model: 'cbz', cc: 150 }
```

- **4.loop over array of mixed data types**

```js
Expected Output =
introducing bike
{ brand: 'honda', model: 'cbz', cc: 150 }
2024
null
true
```

```js
const mixedArr = [
  "introducing bike",
  { brand: "honda", model: "cbz", cc: 150 },
  2024,
  null,
  true,
];
for (let index = 0; index < mixedArr.length; index++) {
  const element = mixedArr[index];
  console.log(element);
}
//output =
//introducing bike
//{ brand: 'honda', model: 'cbz', cc: 150 }
//2024
//null
//true
```

## Object

- looping over keys
- **1. loop over the only keys in the obj.**

```js
Expected Output =
brand;
model;
cc;
```

```js
const obj = { brand: "honda", model: "cbz", cc: 150 };
const objArr = Object.keys(obj);
for (let index = 0; index < objArr.length; index++) {
  const element = objArr[index];
  console.log(element);
}

//output =
//brand;
//model;
//cc;
```

// lopping over values

- **2. loop over the only values in the obj.**

```js
Expected Output =
honda;
cbz;
150;
```

```js
const obj = { brand: "honda", model: "cbz", cc: 150 };
const objArr = Object.values(obj);
for (let index = 0; index < objArr.length; index++) {
  const element = objArr[index];
  console.log(element);
}

//output =
//honda;
//cbz;
//150;
```

- using two array
- **3.looping over key and value of an object**

```js
Expected output =
fullName : salman khan
age : 50
isMarried : false
city : mumbai
```

```js
//method 1 using two arrays
const salman = {
  fullName: "salman khan",
  age: 50,
  isMarried: false,
  city: "mumbai",
};

const keys = Object.keys(salman);
const values = Object.values(salman);
for (let index = 0; index < keys.length; index++) {
  const key = keys[index];
  const value = values[index];
  console.log(`${key} : ${value}`);
}
```

- using single array and object itself

```js
//method 2 using single array
expected output =
salman khan
fullName : salman khan
age : 50
isMarried : false
city : mumbai
```

```js
const salman = {
  fullName: "salman khan",
  age: 50,
  isMarried: false,
  city: "mumbai",
};

const hi = salman.fullName;
console.log(hi);
const keys = Object.keys(salman);

for (let index = 0; index < keys.length; index++) {
  const key = keys[index];
  console.log(key, ":", salman[key]);
}

//output =
//salman khan
//fullName : salman khan
//age : 50
//isMarried : false
//city : mumbai
```
