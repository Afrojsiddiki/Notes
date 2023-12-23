#loop

```js
loop formate =
for (let i = 0; i < item.length; i++) {
  console.log();
}
```

```js
 [ to search words in array]
const bikes = ["dominar", "ns", "pulsar", "discover"];
const wordToFind = "ns";

let isFound = false;

for (let i = 0; i < bikes.length; i++) {
  const item = bikes[i];
  if (item === wordToFind) {
    isFound = true;
  }
}

if (isFound) {
  console.log("Word exist in the sentence.");
} else {
  console.log("Word does not exist.");
}

```
