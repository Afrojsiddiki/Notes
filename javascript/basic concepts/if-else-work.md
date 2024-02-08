###Result of exam

```js
const examMark = 80;

if (examMark === 100) {
  console.log("Congrats, you've scored full mark");
}

if (examMark > 80) {
  console.log("Distinction++");
}

if (examMark === 80) {
  console.log("Just Distinction");
}

if (examMark >= 60) {
  console.log("First Division");
}

if (examMark >= 40) {
  console.log("Pass");
}

if (examMark < 40) {
  console.log("fail");
}
```

```js
if (examMark === 100) {
  console.log("Congrats, you've scored full mark");
} else if (examMark > 80) {
  console.log("Distinction++");
} else if (examMark === 80) {
  console.log("Just Distinction");
} else if (examMark >= 60) {
  console.log("First Division");
} else if (examMark >= 40) {
  console.log("Pass");
} else {
  console.log("Fail");
}
```
