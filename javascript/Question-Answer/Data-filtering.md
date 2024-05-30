## DATA FILTERING(deleting)

- **Removing Unwanted data from the OriginaL data.**

**1. Remove the duplicate from the above result. (Data Filtering)**

```js
const expectedOutput = ["gmail", "outlook", "yahoo"];
```

```js
// Solution 1
const emails = [
  "er.firojsiddiki@gmail.com",
  "mr.afrojsiddiki@gmail.com",
  "firojvsfacebook@outlook.com",
  "info@yahoo.com",
];
const domains = [];
for (let i = 0; i < emails.length; i++) {
  const item = emails[i];
  const result = item.split("@");
  const resultLastItem = result[result.length - 1];
  const dotSplits = resultLastItem.split(".  ");
  const serviceProvider = dotSplits[0];
  domains.push(serviceProvider);
}

console.log(domains); //[ 'gmail', 'gmail', 'outlook', 'yahoo' ]

resultt.shift();
console.log(resultt); //[ 'gmail', 'outlook', 'yahoo' ]
```

**2. Find the maximum temperature from the array.(Data filtering)**

```js
const expectedOutput: 28
```

```js
// Solution 2 using loop
const temperatures = [18, 22, 25, 20, 15, 28];

let max = 0;
for (let i = 0; i < temperatures.length; i++) {
  let item = temperatures[i];
  if (item > max) {
    max = item;
  }
}
console.log("maximum temperatures = ", max); //maximum temperatures = 28
```

**3. Generate a new array with books having more than 250 pages.(Data Filtering)**

```js
const expectedOutput: [{id: 2, title: 'Book 2', author: 'Author 2', pages: 300}]
```

```js
const books = [
  {
    id: 1,
    title: "Book 1",
    author: "Author 1",
    pages: 200,
  },
  {
    id: 2,
    title: "Book 2",
    author: "Author 2",
    pages: 300,
  },
  {
    id: 3,
    title: "Book 3",
    author: "Author 3",
    pages: 250,
  },
];

let newBooks = [];
for (let i = 0; i < books.length; i++) {
  let book = books[i];
  if (book.pages > 250) {
    newBooks.push(book);
  }
}
console.log(newBooks);
// [ { id: 2, title: 'Book 2', author: 'Author 2', pages: 300 } ]
```

**4. Generate a new array with order IDs having total greater than 60.(Data filtering)**

```js
const expectedOutput: [2, 3]
```

```js
const orderList = [
  { id: 1, total: 50 },
  { id: 2, total: 70 },
  { id: 3, total: 90 },
];

let resultOrderList = [];
for (let i = 0; i < orderList.length; i++) {
  let item = orderList[i];
  if (item.total > 60) {
    resultOrderList.push(item.id);
  }
}
console.log(resultOrderList);
//[2,3]
```

**5. Count the occurrences of each fruit in the array.(Data Filteration)**

```js
const expectedOutput: { Apple: 2, Banana: 1, Orange: 1, Mango: 1 }
```

```js
const fruits = ["Apple", "Banana", "Orange", "Apple", "Mango"];

let fruitsCountt = {};
for (let i = 0; i < fruits.length; i++) {
  let fruitItem = fruits[i];
  let fruitsCount = 0;
  for (let j = 0; j < fruits.length; j++) {
    let fruitItem2 = fruits[j];
    if (fruitItem === fruitItem2) {
      fruitsCount++;
    }
    fruitsCountt[fruitItem] = fruitsCount;
  }
}
console.log(fruitsCountt);
//["Apple", "Banana", "Orange", "Apple", "Mango"]
```

**6. find the item counts of items array.(Data filtering)**

```js
const ExpectedOutputt = {
  Apple: 3,
  Banana: 3,
  Orange: 1,
  Mango: 1,
  Gauva: 1,
  Grapes: 1,
};
```

```js
const items = [
  "Apple",
  "Banana",
  "Orange",
  "Apple",
  "Mango",
  "Banana",
  "Banana",
  "Gauva",
  "Apple",
  "Grapes",
];

let itemCountt = {};
for (let i = 0; i < items.length; i++) {
  let Item = items[i];
  let Count = 0;
  for (let j = 0; j < items.length; j++) {
    let Item2 = items[j];
    if (Item === Item2) {
      Count++;
    }
    itemCountt[Item] = Count;
  }
}
console.log(itemCountt);
//{ Apple: 3, Banana: 3, Orange: 1, Mango: 1, Gauva: 1, Grapes: 1 }
```

**7.find the object contains duplicate or not.(Data filtering)**

```js
 logic: if any of the items of the itemCount object is greater than 1, then it contains duplicate.
```

```js
//true
```

```js
const items = [
  "Apple",
  "Banana",
  "Orange",
  "Apple",
  "Mango",
  "Banana",
  "Banana",
  "Gauva",
  "Apple",
  "Grapes",
];
let hasDuplicate = false;
const counts = Object.values(itemCountt);
for (let i = 0; i < counts.length; i++) {
  const count = counts[i];
  if (count > 1) {
    hasDuplicate = true;
    break;
  }
}

console.log({ hasDuplicate }); //true
```

**8. find and remove the duplicate from the array.(Data filtering)**

```js
const items = [
  "Apple",
  "Banana",
  "Orange",
  "Apple",
  "Mango",
  "Banana",
  "Banana",
  "Gauva",
  "Apple",
  "Grapes",
];
for (let i = 0; i < items.length; i++) {
  let Item = items[i];
  let isDup = false;
  for (let j = 0; j < items.length; j++) {
    let Item2 = items[j];
    if (Item === Item2) {
      isDup = true;
      break;
    }
  }
  if (!isDup) {
    noDuplicate.push(Item);
  }
}
console.log(noDuplicate);
```

// find item count in an array
