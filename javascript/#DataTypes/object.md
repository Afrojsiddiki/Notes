#object

-- **it is a type of datatypes which can store multiple keys and values in it .**

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

**CRUD**

```js
`const user = {
name: "afroj siddiki",
class: 12,
age: 20,
ismale: true,
color: "brown",
};` **create**
`console.log(user); ` **read**
`user.age = 18;` **update**
`user.religion = "muslim";` **update**
`console.log(user); `**read**
`delete user.color; `**delete** , **update**
`console.log(Object.keys(user)); `**read**
`console.log(Object.values(user));` **read**
`const values = Object.values(user); **create**
```

- concetp of ascessing Array of anobject

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

```js

###functions related objects :

- `user.key = value` [ to add new keys and value of an object]
- `delete object.key` [ to delete keys and value of an object ]
- `Object.keys(object)` [ to print the only keys of an object in an array ]
- `Object.values(object)` [ to print the only vaules of an object in an array ]
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
