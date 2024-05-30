##DATA AGGREGATION

- **The process of taking out the result by processing the different data id data aggregation.**

**1. Calculate the total expenses from the array.(Data Aggegration)**

```js
const expectedOutput: 1000
```

```js
const expenses = [100, 200, 150, 300, 250];
let total = 0;
for (let i = 0; i < expenses.length; i++) {
  let expense = expenses[i];
  total = total + expense;
}
console.log(total);

//output = 1000
```
