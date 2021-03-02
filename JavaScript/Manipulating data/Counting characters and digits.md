# Counting Characters and Digits 

_Use the .length property._


## Counting letters of a word 

```JS

let word = "Paralelepipedo"
console.log(word.length)    ----->    14  

```


## Counting digits of a number

```JS 

let number = 12345
console.log(number.length)    ----->    It is Undefined, because a numberic data can not receive the property `.length` . So, we must convert the numberic data into a string data.

That is,

console.log(String(number).length)    ----->    5 

```
