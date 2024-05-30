#object

-- **it is a type of datatypes which can store multiple keys and values in it .**

- . operator is used to access static key of an object [per-known or hard coded]

- Of operator is used to access dynamic key of an object ["***"]

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

//data mutate.
//Data mutation is considered as bad practise oftenly because it does not preserve old data.
//Original data is lost forever.
//it could create hard to find bug.
```

- **Concept of objects**

```js
const object1 = {}; // created a variable of type object.
const name = "Afroj";
// const students = ["Afroj", "Firoj", "Saharoj", "Sakina", "Soyaib"];
Object.keys(object); // to print keys of object in array
Object.values(object); // to print values of object in array
object1.afroj = siddiki; // push direct keys and values
object[keys] = values; //push variable in an object

const student1 = {
  firstName: "Afroj",
  hometown: "parasi",
  profession: "bussinessman",
  age: 20,
  isMale: true,
  brothers: ["Firoj", "Sahu"],
};

const student2 = {
  name: "Firoj",
  hometown: "parasi",
  profession: "bussinessman",
  age: 20,
  isMale: true,
  brothers: ["Afroj", "Sahu"],
};

console.log([student1, student2]);

const keys = Object.keys(student1);
const values = Object.values(student1);
console.log(keys); //[ 'firstName', 'hometown', 'profession', 'age', 'isMale', 'brothers' ]

console.log(values); //[ 'Afroj', 'parasi', 'bussinessman', 20, true, [ 'Firoj', 'Sahu' ] ]

for (let i = 0; i < values.length; i++) {
  const item = values[i];
  if (typeof item === "string") {
    console.log(item.toUpperCase());
    //AFROJ
    //PARASI;
    // BUSSINESSMAN;
    //20;
    //true;
  } else {
    console.log(item); //[ 'Firoj', 'Sahu' ]
  }
}
```

```js
// create
let bottle = {
  color: "black",
  brand: "slimline",
  type: "thermas",
  material: "metal",
};

const key1 = "design";
const value1 = "plain";

console.log(bottle); // read
// bottle = null; // delete

//result : bottle = {
//  color: "black",
//  brand: "slimline",
//  type: "thermas",
//  material: "metal",
// };

console.log(bottle.brand);
console.log(bottle["brand"]); //of operator acess
//result= slimline

// console.log(bottle["brand"]);
// bottle.brand = "tata"; // property update
bottle["brand"] = "tata";
console.log(bottle["brand"]); // tata

// bottle.shape = "cylinder";
bottle["shape"] = "cylinder";
bottle[key1] = value1; //pushing by of operator
delete bottle.type;

console.log(bottle);
// result : {
//  color: 'black',
//  brand: 'tata',
//  material: 'metal',
//  shape: 'cylinder',
//  design: 'plain'
// }
```

```js
//print keys and values of object
const shoaib = {
  name: "shoaib siddiki",
  age: 20,
  rollno: 1,
  homeTown: "bhairawha",
  isMale: true,
  bankBalance: undefined,
};

//print keys and values of object
const shoaib = {
  name: "shoaib siddiki",
  age: 20,
  rollno: 1,
  homeTown: "bhairawha",
  isMale: true,
  bankBalance: undefined,
};

const keys2 = Object.keys(shoaib);
const values2 = Object.values(shoaib);
console.log(keys2); //[ 'name', 'age', 'rollno', 'homeTown', 'isMale', 'bankBalance' ]
console.log(values2); //[ 'shoaib siddiki', 20, 1, 'bhairawha', true, undefined ]
```

**CRUD OPERATION ON AN OBJECT**
[ ] operator to access value using dynamically key (key i.e stored in variable)

```js
///create
const item1 = "value2";

const student = {
  fullName: "Afroj siddiki",
  town: "parasi",
  age: 20,
  rollno: 2,
  item1,
};

//read whole object
console.log("whole object =", student);
//whole object = {
//  fullName: 'Afroj siddiki',
//  town: 'parasi',
//  age: 20,
//  rollno: 2,
//  item1: 'value2'
// }

//read value by key
console.log("value by key =", student.fullName);
// result :
//value by key = Afroj siddiki

//read all keys only
console.log("keys only =", Object.keys(student));
//keys only = [ 'fullName', 'town', 'age', 'rollno', 'item1' ]

//read all vaules
console.log("values only =", Object.values(student));
//values only = [ 'Afroj siddiki', 'parasi', 20, 2, 'value2' ]

//update
student.religion = "muslim";

//#DELETE
delete student.rollno;
console.log("deleted rollno =", student);
//deleted rollno = { fullName: 'Afroj siddiki', town: 'parasi', age: 20, item1: 'value2' }

//update keys and value in an object
student.classTeacher = "sanjay";
console.log("updating clasTeacher =", student);
//updating clasTeacher = {
// fullName: 'Afroj siddiki',
// town: 'parasi',
//  age: 20,
//  item1: 'value2',
//  classTeacher: 'sanjay'
// }

Object.seal(student);
student.fullName = "firoj siddiki";
console.log(student);
// {
// fullName: 'Afroj siddiki',
// town: 'parasi',
//  age: 20,
//  item1: 'value2',
//  classTeacher: 'sanjay'
// }
```

**CRUD example**

```js
const user = {
name: "afroj siddiki",
class: 12,
age: 20,
ismale: true,
color: "brown",
};` **create**
console.log(user);  **read**
user.age = 18; **update**
user.religion = "muslim"; **update**
console.log(user); **read**
delete user.color; **delete** , **update**
console.log(Object.keys(user)); **read**
console.log(Object.values(user)); **read**
const values = Object.values(user); **create**
```

```js

###functions related objects :

- `user.key = value` [ to add new keys and value of an object]
- `delete object.key` [ to delete keys and value of an object ]
- `Object.keys(object)` [ to print the only keys of an object in an array ]
- `Object.values(object)` [ to print the only vaules of an object in an array ]
```

- **concetp of ascessing Array of anobject**

```js
const shoaib = {
  name: "shoaib siddiki",
  age: 20,
  rollno: 2,
  homeTown: "bhairawha",
  isMale: true,
  bankBalance: 5000,
};

const keys = Object.keys(shoaib);
const values = Object.values(shoaib);
console.log(keys);
console.log(values);

const keyName = "name";
console.log(keyName, ":", shoaib[keyName]);

`output :
 [ 'name', 'age', 'rollno', 'homeTown', 'isMale', 'bankBalance' ]
[ 'shoaib siddiki', 20, 2, 'bhairawha', true, 5000 ]`;
```

- **loop on an object**

```js
const salman = {
  fullName: "salman khan",
  age: 50,
  isMarried: false,
  city: "mumbai",
};
let newSalman = [];
const salmanKeys = Object.keys(salman);
const salmanValues = Object.values(salman);
for (let index = 0; index < salmanKeys.length; index++) {
  const element = salmanKeys[index];
  const element2 = salmanValues[index];
  let save = [element, element2];
  newSalman.push(save);
}
console.log(newSalman);

//[
//[ 'fullName', 'salman khan' ],
//[ 'age', 50 ],
//[ 'isMarried', false ],
//[ 'city', 'mumbai' ]
//]
```

- **convert the object into array of array then convert it into object.**

```js
//expected output: array of array
//[
//["fullName", "salman khan"],
//["age", 50],
// ["isMarried", false],
// ["city", "mumbai"],
//];

const salman = {
  fullName: "salman khan",
  age: 50,
  isMarried: false,
  city: "mumbai",
};
let newSalman = [];
const salmanKeys = Object.keys(salman);
const salmanValues = Object.values(salman);
for (let index = 0; index < salmanKeys.length; index++) {
  const keys = salmanKeys[index];
  const values = salmanValues[index];
  let save = [keys, values];
  newSalman.push(save);
}
console.log(newSalman);

//output:
//[
//["fullName", "salman khan"],
//["age", 50],
// ["isMarried", false],
// ["city", "mumbai"],
//];

//expected output of array of array to an object =
//{ fullName: 'salman khan', age: 50, isMarried: false, city: 'mumbai' }

const newSalmanObj = {};
for (let index = 0; index < newSalman.length; index++) {
  let [element, element2] = newSalman[index];
  newSalmanObj[element] = element2;
}
console.log(newSalmanObj);
//{ fullName: 'salman khan', age: 50, isMarried: false, city: 'mumbai' }
```

```js
const hero = {
  name: "salman khan",
  age: 50,
  brother: "arbaaz khan",
  Ismarried: false,
};

const heroKeys = Object.keys(hero); //converted to array of key
const heroValues = Object.values(hero); //converted to array of value

console.log(`hero keys = ${heroKeys}`);
console.log(`hero values = ${heroValues}`);

//print the key & value to an array of array
const heroKeysAndValues = [];
for (let i = 0; i < heroKeys.length; i++) {
  let key = heroKeys[i];
  let value = heroValues[i];
  let heroData = [key, value];
  heroKeysAndValues.push(heroData);
}
console.log(heroKeysAndValues);

// convert key & value oo an array of array to object
const newhero = {};
for (let i = 0; i < heroKeysAndValues.length; i++) {
  let [key, value] = heroKeysAndValues[i];
  newhero[key] = value;
  sn = i + 1;
}
console.log(newhero);
```

```js
###loop on an object :

` for (let i = 0; i < values.length; i++) {
  const item = values[i];
  if (typeof item === "string") {
    console.log(item.toUpperCase());
  } else {
    console.log(item);
  }
}`

: this loop is to print all the values of an object touppercase .

```
