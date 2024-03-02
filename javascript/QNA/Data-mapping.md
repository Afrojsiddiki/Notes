##DATA MAPPING (find)

- **The process of connecting data of from variable to find one data from one table to another table.**

##QNA

**1. Replace the id ot he students from classrom array with their respective object from students.(Data Mapping)**

```js
Expected Output = {
  grade: '10',
  classTeacher: 'Ramesh',
  students: [ 'afroj', 'safroj', 'kafroj', 'rafroj' ],
  total: 4
}
```

```js
const students = [
  {
    id: 1,
    name: "afroj",
    roll: "22",
  },
  {
    id: 2,
    name: "safroj",
    roll: "23",
  },
  {
    id: 3,
    name: "kafroj",
    roll: "25",
  },
  {
    id: 4,
    name: "rafroj",
    roll: "26",
  },
];

const classroom = {
  grade: "10",
  classTeacher: "Ramesh",
  students: [3, 4, 2, 1],
  total: 4,
};

const classroomObj = classroom.students;
let result = [];

for (let i = 0; i < students.length; i++) {
  const obj = students[i];
  for (let j = 0; j < classroomObj.length; j++) {
    const obj2 = classroomObj[j];
    if (obj.id === obj2) {
      result.push(obj.name);
    }
  }
}
// console.log(result);
classroom.students = result;
console.log(classroom);

// output
//{
//  grade: '10',
//  classTeacher: 'Ramesh',
//  students: [ 'afroj', 'safroj', 'kafroj', 'rafroj' ],
//  total: 4
//}
```
