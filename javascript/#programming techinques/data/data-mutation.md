####Data mutation

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

: it makes changes in the original data store in an varaible .

```js
let intro = "My name is Afroj. I live in kathmandu.";
console.log("intro", intro); //My name is Afroj. I live in kathmandu.
intro = intro.slice(11, 16); // mutation (it only kept the data between the index 11 to 16)

console.log(intro); //afroj
console.log("intro", intro); //afroj
```

```js
let animals = ["Dog", "Cat", "Goat", "Ship", "Rat"];
const petAnimals = [animals[0], animals[1]]; //result = ["dog","cat"]

// no mutation ( it copies the data  of index to new variable)
```

```js
let animals = ["Dog", "Cat", "Goat", "Ship", "Rat"];

animals.splice(2, 5); // matation direct change into var
const petAnimals = animals.slice(0, 2);
console.log(petAnimals);//["dog","cat"]
console.log(animals);//["dog","cat"]

: mutated the data because it chnage the original var

```
