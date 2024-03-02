##Collection of functions

- getTrueCopyOfArray

```js
function getTrueCopyOfArray(array) {
  const result = [];
  for (let i = 0; i < array.length; i++) {
    const item = array[i];
    result.push(item);
  }
  return result;
}
```

- check truthy falsy vaule

```js
function getTruthyFalsy(data) {
  if (data) {
    return true;
  } else {
    return false;
  }
}
```

- print data

```js
function print(data) {
  console.log(data);
}
```

- get detail by name

```js
function getDetailByName(array) {
  let result = {};
  for (let i = 0; i < array.length; i++) {
    const item = array[i];
    const name = item.name;
    if (name === "afroj siddiki") {
      result = item;
    }
  }
  return result;
}
```

- count word of an Array

```js
function countWordInArray(array, wordToCount) {
  let wordCount = 0;
  for (let i = 0; i < array.length; i++) {
    const item = array[i];
    if (item === wordToCount) {
      wordCount++;
    }
  }
  return wordCount;
}
```

- get infoby keys of object

```js
function getInfoByKeys(array) {
  let resultt = {};

  for (let i = 0; i < array.length; i++) {
    const item = array[i];
    const value = student[item];
    resultt[item] = value;
  }
  return resultt;
}
```

