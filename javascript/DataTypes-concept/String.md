# String

-[ **Emptystring is falsy , other strings are truthy** 1]

- It is a data type which can have any character of keyboard like alphabets, numbers or whatever you can type inside String literal "".

- It is created using in the following ways:

  - singlequote string: `''`
    ```js
    const name = "Afroj";
    const intro = 'I'm Afroj' // it is wrong
    ```
  - doublequote string: `""`

    ```js
    const name = "Afroj";
    const intro = "I'm  Afroj";
    ```

  - template string: ``
    ```js
    const name = `Afroj`;
    const intro = `I'm ${name}`;
    ```

- CRUD function of string

  ```js
  let intro = "i am afroj siddiki"; // creating boys string or assigning string data to intro varialble
  const Ichar = intro.charAt(0); // accessing char of intro at 0 index
  intro = "i am firoj siddiki"; //  re-assigning to intro to update intro variable with new string data.
  into = ""; // deleting var
  ```

- **Functions available on strings**

  - `indexOf(sub-string)` : It is used to find index of a substring of a string
  - `toUpperCase()`: It converts string to upper case letters
  - `toLowerCase()`: It converts any string to lower case letters
  - `split(delimter)`: It splits string based on any delimeter like backspace, @, any character, any word, underscore, hyphens etc.
  - `charAT()` : it shows the character of a index in a string

  ```js
  // Examples
  const intro =
    "Hello World ! I'm Learning Javascript. I want to be a developer.";
  const indexOfWantWord = intro.indexOf("want"); //  41
  const upperLetters = intro.toUpperCase(); // HELLO WORLD ! I'M LEARNING JAVASCRIPT. I WANT TO BE A DEVELOPER.
  const lowerLetters = intro.toLowerCase(); // hello world ! I'm learning javascript. i want to be a developer.
  const delimeter = " ";
  const introWords = intro.split(delimeter); // [ "Hello", "World", "!",  "I'm", "Learning", "Javascript.", "I", "want", "to", "be", "a", "developer." ]
  const nameThirdLetter = chatAt(5); // if name is afroj then result is j
  ```

- **CRUD Operation in string**

```js
// CREATING
let intro = "i am afroj siddiki";

// #READ
//printing intro
console.log("Intro = ", intro); // Intro = "i am afroj siddiki"

//Count length of a string
const length = intro.length;
console.log("Lenght of a string = ", length); //Lenght of a string = 18

//printing last character of a string
// console.log(intro.lastIndexOf(""));

//printing the character by indexing using charAt()
console.log("printing character at 0 index = ", intro.charAt(0)); //printing character at 0 index = i

//replacing substring by replace()
const mystring = "hello i am afroj siddiki";
const updateMystring = mystring.replace("afroj", "firoj");
console.log("replacing afroj by firoj = ", updateMystring); //replacing afroj by firoj =  hello i am firoj siddiki

//#UPDATE

//uppercase-lowercase
intro = "i am firoj siddiki";
console.log("uppercase =", intro.toUpperCase()); // uppercase = I AM FIROJ SIDDIKI
console.log("lowercase = ", intro.toLowerCase()); //lowercase =  i am firoj siddiki

//joining multiple string with concat
const string1 = "hello i am afroj .";
const string2 = "i am from parasi .";
const string3 = string1.concat(string2);
console.log("joining multiple string = ", string3);
// result = "hello i am afroj .i am from parasi ."

//extract sub-string
const info = " hello world afroj";
const newinfo = info.substring(12, 18);
// console.log(info); //afroj
console.log("extracting substring by indexing =", newinfo);

//reverse string [converting into array]
var stringg = "hello";
var splitString = "hello".split("");
console.log(splitString); //result [ 'h', 'e', 'l', 'l', 'o' ]
var reverseArray = splitString.reverse();
console.log(reverseArray); //result[ 'o', 'l', 'l', 'e', 'h' ]
var joinArray = reverseArray.join("");
console.log(joinArray); //result = olleh

//adding substring in a string by slice
let orgString = "lovehate";
console.log("originalString = ", orgString);
let addString = "for";
let newString = orgString.slice(0, 4) + addString + orgString.slice(4);
console.log("string added a new substring = ", newString); //"loveforhate"

//trauncate a string (limiting a string character)
var lengthh = 5;
var fullName = "afroj siddiki";
var mytrauncatedString = fullName.substring(0, lengthh);
console.log(mytrauncatedString); //result = afroj

//#DELETE
//deleting string or assigning a empty string
var love = "i love you";
love = "";
console.log(love); //""

//replace method
var name = "manish";
var result = name.replace("manish", "");
// console.log(name);
console.log("making string empty = ", result);
```

- **loop to ascess all items of a string**

```js
let shoaibStr = "shoaib sid";
let shoaibArr = shoaibStr.split(""); // converted to array
console.log(shoaibArr);
for (let i = 0; i < shoaibArr.length; i++) {
  let item = shoaibArr[i];
}
console.log(item);
//result =

//s
//h
//o
//a
//i
//b

//s
//i
//d
```

- **Loop-operation over string character**

```js
const me = "i am afroj siddiki";
for (let i = 0; i < me.length; i++) {
  let char = me.charAt(i);
  console.log(char);
}
//result
// i

//  a
//  m

//  a
//  f
//  r
//  o
//  j

//  s
//  i
//  d
//  d
//  i
//  k
//  i
```
