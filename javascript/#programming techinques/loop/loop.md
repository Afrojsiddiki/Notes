#loop

- for loop structure

```js
for (let i = 0; i < item.length; i++) {
  console.log();
}
```

- print number 1 to 100

```js
let numberLessThanHundred = [];
for (let i = 1; i <= 100; i++) {
  numberLessThanHundred.push(i);
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

##concept of running loop inside loop

**print user with their bankbalance data**

```js
const users = [
  { userId: 1, name: "Firoj" },
  { userId: 2, name: "Sajar" },
  { userId: 12, name: "Afroj" },
  { userId: 202, name: "Sakina" },
  { userId: 20222, name: "Sakina" },
];

const usersBankBalance = [
  { userId: 1, bankBalance: 1000 },
  { userId: 20012, bankBalance: 3000 },
  { userId: 2023, bankBalance: 4000 },
  { userId: 2022, bankBalance: 5000 },
  { userId: 202, bankBalance: 5500 },
  { userId: 2021, bankBalance: 6600 },
  { userId: 12, bankBalance: 3600 },
  { userId: 2, bankBalance: 36000 },
];

const result = [];
// outer loop
for (let i = 0; i < users.length; i++) {
  const userItem = users[i];
  // inner loop
  for (let j = 0; j < usersBankBalance.length; j++) {
    const userBankBalanceItem = usersBankBalance[j];

    if (userItem.userId === userBankBalanceItem.userId) {
      const newData = {
        name: userItem.name,
        bankBalance: userBankBalanceItem.bankBalance,
      };
      result.push(newData);
    }
  }
}

console.log(result);
```
