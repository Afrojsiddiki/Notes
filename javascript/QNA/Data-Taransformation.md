##DATA_TRANSFORMATION

- **The process of visiting the data and deriving the required data from it in any datatypes is data transformation.**

##QNA

**1. Create a new data with husband and wife full name and thier total income together. (Data Transformation)**

```js
const expectedOutput = [
  { husband: "Abhisek Bachhan", wife: "Aiswaray Rai", income: 68899000 },
];
```

```js
// solution
const actors = [
  {
    firstName: "Abhishek",
    lastName: "Bachhan",
    age: 50,
    sex: "male",
    wife: "101",
    salary: 501011,
  },
  {
    firstName: "Salman",
    lastName: "Khan",
    age: 55,
    sex: "male",
    wife: "120",
    salary: 303030,
  },
  {
    firstName: "Ranvir",
    lastName: "kapoor",
    age: 45,
    sex: "female",
    wife: "333",
    salary: 666666,
  },
];
const spouse = [
  {
    id: "101",
    firstName: "Aaiswaray",
    lastName: "Rai",
    age: 55,
    salary: 10000,
  },
  {
    id: "102",
    name: "Katrina kaif",
    firstName: "Kaitrina",
    lastName: "Kaif",
    age: 45,
    salary: 150000,
  },
  {
    id: "120",
    name: null,
    age: null,
    salary: 20000,
  },
  {
    id: "333",
    firstName: "Aaliya",
    lastName: "Bhatt",
    age: 35,
    salary: 300000,
  },
  {
    id: "422",
    firstName: "Madhuri",
    lastName: "Dixit",
    age: null,
    salary: 340000,
  },
];
// create a new data with wife nameinstead     of wife key in actors array;
// create a new data with total income ofa     jodie
// expected output [{husband:'Abhisek    Bachhan', wife:'Aiswaray Rai', income:    68899000}]
let coupleCombinedDetail = [];
for (let i = 0; i < actors.length; i++) {
  const actorsDetail = actors[i];
  for (let j = 0; j < spouse.length; j++) {
    const spouseDetail = spouse[j];
    if (actorsDetail.wife === spouseDetail.id) {
      const newData = {
        ...actorsDetail,
        fullName: actorsDetail.firstName + "     " + actorsDetail.lastName,
        salary: actorsDetail.salary + spouseDetail.salary,
        wife:
          spouseDetail.firstName && spouseDetail.lastName
            ? spouseDetail.firstName + " " + spouseDetail.lastName
            : "No wife",
      };
      //       if (!!actorsDetail.wife) {
      //         const newData = {
      //           ...actorsDetail,
      //           fullName:actorsDetail.    firstName + " " +actorsDetail.    lastName,
      //           salary:actorsDetail.    salary +spouseDetail.salary,
      //           wife: spouseDetail.   firstName + " " + spouseDetail.   lastName,
      //         };
      //       }
      coupleCombinedDetail.push(newData);
    }
  }
}
console.log("couple combined detail=", coupleCombinedDetail);
```

**2. Generate a new array with each number multiplied by 2. (Data Transformation)**

```js
const expectedOutput = [20, 40, 60, 80, 100];
```

```js
// Solution
let numbersMultipliedByTwo = [];
for (let i = 0; i < numbers.length; i++) {
  let num = numbers[i];
  numbersMultipliedByTwo.push(num * 2);
}
console.log(numbersMultipliedByTwo);

const cashFlows = [
  {
    id: 1,
    income: 10000,
    expense: 5000,
  },
  {
    id: 2,
    income: 30000,
    expense: 44400,
  },
  {
    id: 5,
    income: 53000,
    expense: 54400,
  },
];
```

**3. Generate a new data with Net and status using cashFlows. (Data Transformation)**

```js
const expectedOutput = [{ id: 1, net: 50000, status: "profit" }];
```

```js
// Solution
let newCashFlowData = [];
for (let i = 0; i < cashFlows.length; i++) {
  let newData = {};
  let data = cashFlows[i];
  newData = {
    id: data.id,
    net: data.income - data.expense,
    status: newData.net > 0 ? "profit" : "loss",
  };

  newCashFlowData.push(newData);
}
console.log(newCashFlowData);
```

**4. Find out the an array of service provider for the above array.(Data Transformation)**

```js
const expectedOutput = ["gmail", "gmail", "outlook", "yahoo"];
```

```js
// Solution
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

console.log(domains);
```

**5.Generate a new array with 2 rupees discounted prices for each product.(Data transformation)**

```js
const expectedOutput = [
  { id: 1, discountedPrice: 18 },
  { id: 2, discountedPrice: 27 },
  { id: 3, discountedPrice: 22.5 },
];
```

```js
// Solution
const products = [
  {
    id: 1,
    name: "Product 1",
    price: 20,
  },
  {
    id: 2,
    name: "Product 2",
    price: 30,
  },
  {
    id: 3,
    name: "Product 3",
    price: 25,
  },
];

const discountedProduct = [];
for (let i = 0; i < products.length; i++) {
  let newItem = {};
  let productItem = products[i];
  // newItem = {
  //   id: productItem.id,
  //   name: productItem.name,
  //   price: productItem.price - 2,
  // };
  productItem.price = productItem.price - 2;
  discountedProduct.push(newItem);
}
console.log(discountedProduct);
```

**6. tranform the above array data into object.(Data Transformation)**

```js
expected output: {apple:5,mango:10,gauva:0, custard:1}
```

```js
const itemsCount = [
  ["apple", 5], // item and its count
  ["mango", 10],
  ["gauva", 0],
  ["custard", 1],
];
let output = {};

for (let i = 0; i < itemsCount.length; i++) {
  let [fruitName, count] = itemsCount[i];
  output[fruitName] = count;
}
console.log(output);
```

**7. Generate a new array with unique product names from all orders.(Data Transfromation)**

```js
const expectedOutput: ['Product 1', 'Product 2', 'Product 3']
```

```js
const orders = [
  {
    id: 1,
    products: ["Product 1", "Product 2"],
  },
  {
    id: 2,
    products: ["Product 2", "Product 3"],
  },
  {
    id: 3,
    products: ["Product 1", "Product 3"],
  },
];

const ordersResult = [];
for (let i = 0; i < orders.length; i++) {
  let product = 0;
  let newOrders = "";
  let ordersItem = orders[i];
  newOrders = ordersItem = "product";
  ordersResult.push(newOrders);
}
console.log(ordersResult);
```

**8. place the object item into array of array.(Data Transformation)**

```js
const fruits = { apple: 5, mango: 10, gauva: 0, custard: 1 };
let keys = Object.keys(fruits);
let values = Object.values(fruits);

let output = [];
for (let i = 0; i < keys.length; i++) {
  let fruit = keys[i];
  let count = values[i];

  // method 1
  //   const arrayItem = [];
  //   arrayItem.push(key);
  //   arrayItem.push(value);

  // method 2
  //   const arrayItem = [];
  //   arrayItem[0] = key;
  //   arrayItem[1] = value;

  // method 3
  const arrayItem = [fruit, count];

  output.push(arrayItem);
}
console.log(output);
```
