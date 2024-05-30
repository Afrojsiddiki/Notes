````js
**1. Variables (var, let, const) 2. Data Types (string, number, boolean, null, undefined, array, object)
Two Types
-- 1. Primitive data types (unmuatable)
eg: boolean, number, string, null, undefined
-- 4. Complex data types (mutable) - eg: - array, object
let name = "Firoj"** ```


```js
 - loop

 for (initialization; condition; increment) {
    to do
}

const bikes = ["ns", 'tvs', 'hero', "bajaj", "plantina"];
const mixedArray = [100, "firoj", null, true];
const roomNumbers = [302, 102, 402]
const mobiles = ["iphone", "android"];

 for(let i = 0; i < bikes.length; i++) {
   console.log(bikes[i])
}
````

```js
-array(examples);
const bikes = ["ns", "tvs", "hero", "bajaj", "plantina"];
const mixedArray = [100, "firoj", null, true];
const roomNumbers = [302, 102, 402];
const mobiles = ["iphone", "android"];
```

##fizzbuzz program

```js

Exercise
write a program to print FIZZ if a number is divisible by 3 and print FUZZ if a number is divisible by 5 and print FIZZFUZZ if the number is divisible by both.

solution : 1

const num = 15

if(num % 3 === 0 && num % 5 === 0){
  console.log("divisible by 3 and divisible by 5")
  return;
}


if(num % 3 === 0){
  console.log("divisible by 3")
  return;
}

if(num % 5 === 0){
  console.log("divisible by 5")
  return;
}
```

```js
solution: 2;

const numb = 19;
if (numb % 3 === 0 && numb % 5 === 0) {
  console.log("divisible by 3 and 5");
} else if (numb % 3 === 0) {
  console.log("divisible by 3");
} else if (numb % 5 === 0) {
  console.log("divisible by 5");
} else {
  console.log("divisible by neither ");
}
```

[ **Information tempelete program**

```js
const name = "Afroj"
const age = "20"
const gender = "male"
const profession = "student"
const city = "parasi"
const goal = "developer"

console.log(`Me ${name} , of age ${age} , gender ${gender} , i am a ${profession} by profession . i live in ${city} , And my goal is to be a ${goal}.`)

**output /result = Me Afroj , of age 20 , gender male , i am a student by profession . i live in parasi , And my goal is to be a developer.** ]

```

```js
 Replace first a in string with @
1. repacing char with anathor char or words () in a string.


const myIntro = "hello guys, his name is aman";
const start = 'my name is ';
const intro = 'my name is afroj Siddiki.';
const letterToReplace = 'a';
const letterToReplaceWith = '@';
const letterToReplaceIndex = intro.indexOf(letterToReplace); // 4
const start = intro.substring(0, letterToReplaceIndex) // intro.substring(0,4)
const introLength = intro.length;
// console.log(introLength);
const end = intro.substring(letterToReplaceIndex + 1, intro.length) // intro.substring(5,23)
const result33 = start + letterToReplaceWith + end;
// console.log(result33)
const intro2 =  intro.replace('a','@');
const intro3 = intro.replaceAll('a', '@');
```
