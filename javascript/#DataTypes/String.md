# String

-[**Emptystring is falsy , other strings are truthy**]

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

- CRUD on string data

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
  const upperLetters = intro.toLowerCase(); // hello world ! I'm learning javascript. i want to be a developer.
  const delimeter = " ";
  const introWords = intro.split(delimeter); // [ "Hello", "World", "!",  "I'm", "Learning", "Javascript.", "I", "want", "to", "be", "a", "developer." ]
  const nameThirdLetter = chatAt(5); // if name is afroj then result is j
  ```

- Loop-operation

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
