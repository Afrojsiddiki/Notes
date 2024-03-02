```js
// method 1: to loop over object
console.log(`loop on values array will run ${values.length} times`);
for (let i = 0; i < values.length; i++) {
  const valuesItem = values[i];
  const keysItem = keys[i];
  const sn = i + 1;
  console.log(sn, keysItem, ":", valuesItem);
}

const keyName = "name";
console.log(`value of ${keyName} is ${user[keyName]}`);
console.log("value of", keyName, "is", user[keyName]);
```

```js
// method 2: to loop over object
for (let i = 0; i < paritalUserKeys.length; i++) {
  const key = keys[i];
  const value = user[key];
  const sn = i + 1;
  console.log(sn, key, ":", value);
}
```

```js
const paritalUserKeys = ["name", "age"];
for (let i = 0; i < paritalUserKeys.length; i++) {
  const item = paritalUserKeys[i];
  const itemValueFromUserObect = user[item];
  const sn = i + 1;
  console.log(sn, item, itemValueFromUserObect);
}
```
