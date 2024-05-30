# DataTypes

```js
1. string
2. array
3. boolean
4. null
5. undefined
6. number
7. object
8. NaN
```

### Meaning of CRUd operations

**C** = create
**R** = read , view , access , visit
**U** = update , Change , modify
**D** = delete , remove

- **to print any keys with value together dynamically**

`const shoaib = {
name: "shoaib siddiki",
age: 20,
rollno: 2,
homeTown: "bhairawha",
isMale: true,
bankBalance: undefined,
};`

`const keys = Object.keys(shoaib);`
`console.log(keys);`

`const keyName = "age";`
`console.log(keyName, ":", shoaib[keyName]);`

`for (let i = 0; i < shoaib.length; i++) {
const item = shoaib[i];
const valueOfKeysFromShoaib = shoaib[keyName];
console.log(valueOfKeysFromShoaib);
}`
