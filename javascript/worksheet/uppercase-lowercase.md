```js
## toUpperCase

const bikes = [ "dominar" , "ns" , "Pulsar" , "discover", "pulsar220", "Nk" ,"nk200", "pulsar", "Dominar","Pulsar", "ns"]
const wordToFind =  "pulsar";

let isFound = false;

for(let i = 0 ; i < bikes.length ; i++ ){
  const item = bikes[i];
  if(item === wordToFind)
  {isFound = true ;
  }
}

let pulsorCount = 0;
let nsCount = 0;

for(let i = 0 ; i < bikes.length ; i++){
  let item = bikes[i];
  if(item === "pulsar"){
    console.log(item.toUpperCase())
    pulsorCount = pulsorCount + 1
  }
  if(item === "ns"){
    console.log(item.toUpperCase())
    nsCount = nsCount + 1
  }
}

## toLowerCase

const bikes = [ "dominar" , "ns" , "Pulsar" , "discover", "pulsar220", "Nk" ,"nk200", "pulsar", "Dominar","Pulsar", "ns"]
const wordToFind =  "pulsar";

let isFound = false;

for(let i = 0 ; i < bikes.length ; i++ ){
  const item = bikes[i];
  if(item === wordToFind)
  {isFound = true ;
  }
}

let pulsorCount = 0;
let nsCount = 0;

for(let i = 0 ; i < bikes.length ; i++){
  let item = bikes[i];
  if(item === "pulsar"){
    console.log(item.toLowerCase())
    pulsorCount = pulsorCount + 1
  }
  if(item === "ns"){
    console.log(item.toLowerCase())
    nsCount = nsCount + 1
  }
}




  const bikes = [ "dominar" , "ns" , "pulsar" , "discover", "pulsar220", "nk" ,"nk200", "pulsar", "dominar","pulsar", "ns"]

  for(let i = 0 ; i < bikes.length ; i++){
    let item = bikes[i]
    // console.log(bikes[i].toUpperCase())
    console.log(item.toLowerCase())
  }

```
