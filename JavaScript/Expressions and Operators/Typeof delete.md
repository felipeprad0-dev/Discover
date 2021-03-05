# Typeof Delete 

_Both are unary operators._


## Typeof

_Returns a string indicating the type of the operand._

```JS
let num = 1;

console.log(typeof num)     ----->     Number
```       


## Delete

_Removes a given property from an object._

```JS
const person = {
    name: "Felipe",
    age: 25,
    city: "Sao Simao"
}

delete person.age;

console.log(person)     ----->      person {name: "Felipe", city: "Sao Simao"}
```