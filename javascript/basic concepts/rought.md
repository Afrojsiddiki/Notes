```js
1. Variables (var, let, const)
2. Data Types (string, number, boolean, null, undefined, array, object)
Two Types
1. Primitive data types (unmuatable)
eg. - boolean, number, string, null, undefined
2. Complex  data types (mutable)
eg. - array, object
let name = "Firoj"

console.log('My name is', name)
let person = null;
let house = undefined

// console.log(house)

// string data
"Afroj"
"Firoj"
"2490240280@"

// boolean data
true
false

// null data
null

// undefined data
undefined

console.log(prices)

Operations on number data types

const A = 40;
const B = 30
const sum = A + B;
const difference = A - B;
const division = A / 0;
const mul = A * B;
const pow = A ** 2;
console.log('sum', sum);
console.log('diff', difference);

console.log("sum is", sum, "And diff is", difference);

console.log(`sum is ${sum}, diff is ${difference}, division is ${division} and multiplicaton is ${mul} and power is ${pow}`)

OPERATIONS OF STRING DATA TYPES

const snake_case = "afroj_siddiki";
const camelCase = "afrojSiddiki";
const PascalCase = "AfrojSiddiki"

const firstName = "Afroj";
const lastName = "Siddiki";
const money = 5000
// const fullName =  firstName + lastName;
const fullName = firstName + " " + lastName
const result = money + firstName;
// console.log(result)
const fullName = `${firstName} ${lastName}`
console.log(fullName.toUpperCase())

Operations on boolean data types
truthy value and falsy value

const isAdmin = true;
const isStaff = false;
console.log(isAdmin, isStaff)

const myNumber = !132;
console.log(myNumber);

const myString = !Boolean("");
console.log(myString)

console.log(Boolean(null))
console.log(Boolean(undefined))

// object
let prices = {
  momo: 200,
  chowmin: 180,
}

array
const momoList = ["steamMomo", "friedMomo", "kotheyMomo"]

conditional statement

if(false){

}

else{

}

const examMark = 80

if(examMark === 100){
   console.log("Congrats, you've scored full mark");
}

if(examMark > 80){
  console.log("Distinction++")
}

if(examMark === 80){
  console.log("Just Distinction")
}

if(examMark >= 60){
  console.log("First Division")
}

if(examMark >= 40){
  console.log("Pass")
}

if(examMark < 40){
  console.log("fail")
}

if(examMark === 100) {
  console.log("Congrats, you've scored full mark");
}else if(examMark >  80){
  console.log("Distinction++")
}else if(examMark === 80){
  console.log("Just Distinction")
} else if(examMark >= 60){
  console.log("First Division")
}else if(examMark >= 40){
  console.log("Pass")
}else {
  console.log("Fail")
}

const remainder  = 20 % 3;
console.log(remainder);
const myNumber2 = 21;

if(myNumber2 % 3 === 0){
  console.log('divisible by 3')
}else{
  console.log('not divisible by 3')
}

Exercise
write a program to print FIZZ if a number is divisible by 3 and print FUZZ if a number is divisible by 5 and print FIZZFUZZ if the number is divisible by both.

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

const name = "Afroj"
const age = "20"
const gender = "male"
const profession = "student"
const city = "parasi"
const goal = "developer"

console.log(`Me ${name} , of age ${age} , gender ${gender} , i am a ${profession} by profession . i live in ${city} , And my goal is to be a ${goal}.`)

if(condition){
  // todo
}

if(condition){

}else{

}

if(condition){

}else if(condition){

}else if(condition){

}else{

}

const numb = 19
if (numb % 3 === 0 && numb % 5 === 0) {
  console.log("divisible by 3 and 5")
} else if (numb % 3 === 0) {
  console.log("divisible by 3")
} else if (numb % 5 === 0) {
  console.log("divisible by 5")
} else {
  console.log("divisible by neither ")
}

CRUD - Create, Read, Update, Delete
const bikes = ["ns", 'tvs', 'hero', "bajaj", "plantina"];
const mixedArray = [100, "firoj", null, true];
const roomNumbers = [302, 102, 402]
const mobiles = ["iphone", "android"];

const lastIndex = bikes.length - 1;
const lastArrayItem = bikes[lastIndex];
console.log(lastArrayItem);

Replace the last item of an array with named as itemName2
console.log('original bike array', bikes);
const lastItem = bikes[bikes.length - 1];
console.log('lastItem',lastItem);
const newItem = lastItem + "2";
console.log('new item',newItem);
bikes[bikes.length - 1] = newItem
console.log('update bike array', bikes)

console.log(bikes)
syntaxes

declare array: (C)
['item1','item2'];

access array item (R)
array[index]

update (U)
array[index] = 'value'

delete
array.pop()

bikes.pop();
bikes.push('pulsor')
bikes.unshift('pulsor')
console.log(bikes[0]);
console.log(bikes[1])

Replace first a in string with @
1. repacing char with anathor char or words () in a string.

const myIntro = "hello guys, his name is aman";
const start = 'my name is ';
const intro = 'my name is afroj Siddiki.';
const letterToReplace = 'g';
const letterToReplaceWith = '@';
const letterToReplaceIndex = intro.indexOf(letterToReplace); // 4
// const start = intro.substring(0, letterToReplaceIndex) // intro.substring(0,4)
const introLength = intro.length;
// console.log(introLength);
const end = intro.substring(letterToReplaceIndex + 1, intro.length) // intro.substring(5,23)
const result33 = start + letterToReplaceWith + end;
// console.log(result33)
const intro2 = intro.replace('a', '@');
const intro3 = intro.replaceAll('a', '@');

console.log(myIntro.charAt(6));

console.log(intro2);
console.log(intro3)

2. replacing word with another word or char in a string

const intro = 'my name is afroj Siddiki. My brother name is Afroj.';

Loop or iterate

let i = 0;
console.log(i);
// i = i + 1;
i++;
console.log(i);
i = i + 1;
// // i++;
// // console.log(i);
// // i = i + 1;
// // i++;
// // console.log(i);
// // // i = i + 1
// // i++;
// // console.log(i);

// // for (initialization; condition; increment) {
// //    to do
// // }

// // for(let i = 0; i < 100; i++)      {
// //   // console.log(`Afroj is no. ${i}`)
// // }

// // console.log('i value is:', i);

// // console.log(bikes[0])
// // console.log(bikes[1])
// // console.log(bikes[2])
// // console.log(bikes[3])

// // for(let i = 0; i < bikes.length; i++) {
// //   console.log(bikes[i])
// // }

// // console.log(myIntro.charAt(0));
// // console.log(myIntro.charAt(1));
// // console.log(myIntro.charAt(2));

// // for(let i = 0; i < myIntro.length; i++) {
// //   console.log(myIntro.charAt(i));
// // }

// // const marks = ['1', '2', '3', '4', '5','6', '7','8', '9','10']
// // console.log(marks.at(4))

// // let number = 9

// // const remainder = number % 2;
// // console.log('remainder', remainder);

// // const isOddNumber = remainder  === 1; // logic to check odd number
// // console.log('isOddNumber', isOddNumber);

// // if(isOddNumber) {
// //    console.log("it's an odd number")
// //  }

// // for(let i = 0 ;i  <= 10  ; i++ ){
// //   const remainder = i % 2;
// //   const isOddNumber = remainder  === 0; // logic to check odd number
// //   if(isOddNumber) {
// //      console.log(i)
// //    }
// // }

// // problem: find odd number and multiply it by 2
// // expected input: 1, 3, 5, 7, 9
// // expected output: 2, 6, 10, 14, 18

// // for(let number = 0 ; number <= 10; number++){
// //   const isOddNumber = number % 2 === 1
// //   if(isOddNumber) {
// //     console.log(number*2)
// //   }else{
// //     console.log(number)
// //   }

// // }

// // const description = "This is my first programming language";
// // for(let i = 0; i < description.length; i++) {
// //     console.log(description.charAt(i));
// // }
// // print each words of the above description variable;
// // const descriptionWords = description.split(" ")
// // console.log(descriptionWords)

// // for(let i = 0; i < descriptionWords.length; i++) {
// //   console.log(descriptionWords[i]);

// // }

// // const descriptionWithUnderscore = descriptionWords.join("*");
// // console.log(descriptionWithUnderscore);

// // const desc = description.replaceAll(" ", "_");
// // console.log(desc);

// // Array / String
// // C - Create array : const boys = [ "Ram", "shyam"];
// // R - Read/print/view/access/tranverse/visit ex : boys[1]
// // U - Update/Change/Modify boys[1] = "hari"
// // D - Delete/Remove boys.pop()

// //  String
// // C - Create array : const boys = "i am afroj siddiki";
// // R - Read/print/view/access/tranverse/visit ex : boys , i: boys.charAt(0)
// // U - Update/Change/Modify boys = "i am firoj siddiki"
// // D - Delete/Remove = boys = ""

// // 1. manaullly delete item of an array.
// // 2. search an item in an array
// // 3. replace an item from an array with custom item
// // 4. filter items of an array
// // 5. sort an array

// // const me = " i am afroj siddiki"
// // for (let  = 0 ,  < me.length ,i++ )
// //   console.log(me.chartAt(l))
// const me = "i am afroj siddiki"
// const a = 1
// const b = 2
// console.log(me)
// console.log(a + b)
```
