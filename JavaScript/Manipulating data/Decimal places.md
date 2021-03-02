# Decimal Places

_Use `.toFixed(n)` method to fix the decimal places._ 

_Use `.replace()` method to specify what must be changed. ---> `.replace("what", "for what")`_

_When a function is related to an object, we call it `methods`._


## Transforming float numbers with two decimal places

```JS
let number = 453.896547

console.log(number.toFixed(2))      ------>      453.89   

```


## Exchanging periods for commas

```JS

let number = 453.89 

console.log(number.replace(".", ","))      ------>      453,89 

```