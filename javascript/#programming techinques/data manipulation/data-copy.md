##copy method [ assigning new var , ... spered operator]

```js
objects;
// create
// read whole object, value by key, all keys , all values
// delete key
// update key
//  [] operator to access value using dynamically key (key i.e stored in variable)
// . operator to access value using key of the object

// method
// copying primitive and non-primitive data (value and reference)
// mutable and immutable data
// PassByValue and PassByReference
// mutable and immutable function

// data mutate.
// Data mutation is considered as bad practise oftenly because it does not preserve old data.
// Original data is lost forever.
// it could create hard to find bug.
```

- **pass by value or pass by reference**
- **value versus reference(memory address)**
- **What is memory address of a variable**

**imprptant notes :**

- copying a variable data to another variable like below is availble in all primitive datatypes

- copy dont have to mutate org data

```js
const student = ["Ram", "shyam", "hari"];
console.log(student); //result = [ 'Ram', 'shyam', 'hari' ]
const studentCopy = student;
console.log(studentCopy); //result = [ 'Ram', 'shyam', 'hari' ]
```

**How to copy data right way ?**

```js
Two types of data in programming
1. Primitve/old/simple/atomic (string, number, boolean, null, undefined, NaN)
let hobby = "I love programming";
let isAdmin = true;
const bankBalance = 100000;

saving original data before mutating variables
const hobbyCopy = hobby;
const isAdminCopy = isAdmin;
const bankBalanceCopy = bankBalance;

hobby = "I hate ...";
console.log("hobby", hobby);
console.log("hobbyCopy", hobbyCopy);
isAdmin = false;
console.log("isAdminCopy", isAdminCopy);
console.log("isAdmin", isAdmin);

```

2. Non-Primitive/advance/moden/complex (array, object)

```js
const animals = ["Cat", "Dog", "Rat", true, 1000];

const animalsFakeCopy = animals;
const animalsActualCopy = [
  animals[0],
  animals[1],
  animals[2],
  animals[3],
  animals[4],
];

console.log(animalsFakeCopy); //this may bring error internally
console.log(animalsActualCopy); //correct way to copy data
js;

const array = animals; // pass by value or pass by refrence
animalsActualCopy = getTrueCopyOfArray(animals);
animalsActualCopy2 = [...animals];
animals.push("Ranvir");
```

- copy all the data of mordern data types by loop

```js
const animals = ["Cat", "Dog", "Rat", true, 1000];
const animalsActualCopy = [];
for (let i = 0; i < animals.length; i++) {
  const item = animals[i];
  animalsActualCopy.push(item);
}
```

- Example of fake and true copy

```js
const bike = {
  brand: "Bajaj",
  name: "Dominar",
  cc: 400,
  speed: "200kmh",
  accelate() {
    console.log("accelerating");
  },
};

const bikeFakeCopy = bike;
const bikeTrueCopy = { ...bike };

bike.cc = 200;
console.log("bike", bike);
console.log("bikeFakeCopy", bikeFakeCopy);
console.log("bikeTrueCopy", bikeTrueCopy);
```
