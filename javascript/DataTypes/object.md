#object

-- **it is a type of datatypes which can store multiple keys and values in it .**

**CRUD**
`const user = {
name: "afroj siddiki",
class: 12,
age: 20,
ismale: true,
color: "brown",
};` **create**
`console.log(user); ` **read**
`user.age = 18;` **update**
`user.religion = "muslim";` **update**
`console.log(user); `**read**
`delete user.color; `**delete** , **update**
`console.log(Object.keys(user)); `**read**
`console.log(Object.values(user));` **read**
`const values = Object.values(user); **create**

###functions related objects :

- `user.key = value` [ to add new keys and value of an object]
- `delete object.key` [ to delete keys and value of an object ]
- `Object.keys(object)` [ to print the only keys of an object in an array ]
- `Object.values(object)` [ to print the only vaules of an object in an array ]

###loop on an object :

` for (let i = 0; i < values.length; i++) {
  const item = values[i];
  if (typeof item === "string") {
    console.log(item.toUpperCase());
  } else {
    console.log(item);
  }
}`

: this loop is to print all the values of an object touppercase .
