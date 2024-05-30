#Number datatype

- [**0 is false , 1 to infinity is truthy**]
- it is a type of data type which can store any numberic data .

  - it is created by using following ways :

  ```js
  const apple = 150;
  const ball = 10;
  const sum = apple + ball;
  const multiplication = apple * ball;
  const division = apple / ball;
  const power = A ** 2;
  console.log("diff", appple - ball); // result 140
  console.log(sum); // result 160
  ```

  ##CRUD

```js
//#CREATING

var numberArray = [1, 2, 3, 4, 5];

//READING
console.log("printing numberArray = ", numberArray); //result [1, 2, 3, 4, 5]
console.log(" length of numberArray = ", numberArray.length); //result 5
console.log("second number of numberArray = ", numberArray[1]); // result 2

//#UPDATE
//changing third number of the array;
var numberString = numberArray.toString();
console.log("converted array to string", numberString);
var newNumberString = numberString.replace("3", "9");
console.log("changing number of string", newNumberString);
var numberArray = newNumberString.split(","); //changed string to an array
console.log(numberArray);

//adding a new number to the last of the array
numberArray.push("6");
console.log(numberArray);

//#DELETING

//deleting first number of an array
numberArray.shift();
numberArray.unshift(); //to return back the first deleted item
console.log(numberArray);

// deleting last number of an array
numberArray.pop();
console.log(numberArray);
```
