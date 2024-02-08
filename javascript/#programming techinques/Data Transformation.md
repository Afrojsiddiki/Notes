###examples of data transformation :

**transforming data**

```js
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
    firstName: "Ranbir",
    lastName: "Kapoor",
    age: null,
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

const output2 = [];
for (let i = 0; i < spouse.length; i++) {
  item = spouse[i];
  const newData = {
    fullName: item.firstName + "" + item.lastName,
    age: item.age,
    salary: item.salary,
  };
  output2.push(newData);
}
console.log(output2);
```

- write a program to get a list of actors with their fullname and age.

```js
const output = [];

for (let i = 0; i < actors.length; i++) {
  const item = actors[i];
  const newData = {
    // fullName: item.firstName + " " + item.lastName,
    fullName: `${item.firstName} ${item.lastName}`,
    age: item.age,
  };
  output.push(newData);
}

console.log(output);
```

- create a new data with wife name instead of wife key in actors array;

```js
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
    firstName: "Alia",
    lastName: "Bhatt",
    age: 35,
    sex: "female",
    husband: "333",
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
    firstName: "Ranbir",
    lastName: "Kapoor",
    age: null,
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

let actorsDetailWithWifeName = [];

for (let i = 0; i < actors.length; i++) {
  const actorsDetail = actors[i];

  for (let j; j < spouse.length; j++) {
    const spouseDetail = spouse[j];

    if (actorsDetail.wife === spouseDetail.id) {
      const newData = {
        fullName: actorsDetail.firstName + " " + actorsDetail.lastName,
        age: actorsDetail.age,
        sex: actorsDetail.sex,
        salary: actorsDetail.salary,
        wife: spouseDetail.name,
      };
      actorsDetailWithWifeName.push(newData);
    }
  }
}
console.log(actorsDetailWithWifeName);
,,,
```
