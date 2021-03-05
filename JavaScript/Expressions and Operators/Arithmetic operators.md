# Arithmetic Operators

## Sum 
` + ` operator

```JS
console.log(5 + 3)  ----->  8
```


## Subtraction
` - ` operator

```JS
console.log(5 - 3)  ----->  2
```


## Multiplication 
` * ` operator

```JS
console.log(5 * 3)  ----->  15
```


## Division
` / ` operator

```JS
console.log(5 / 3)  ----->  1.6667
```


## Rest of Division 
` % ` operator

```JS
console.log(5 % 3)  ----->  2
console.log(10 % 2)  ----->  0
console.log(21 % 2)  ----->  1
```


## Increment
` ++ ` operator

```JS
let increment = 0;

increment++;
console.log(increment)  ----->  1

increment++;
console.log(increment)  ----->  2
```

Inside the console log is different! If we put `increment++`, it will be 0 because it will only add after this console.log
```JS
let increment = 0;

console.log(increment++)  -----> 0
console.log(increment)  -----> 1
```

If we want to add before, we have to put the operator before the variable
```JS
let increment = 0;

console.log(++increment)  ----->  1
```


## Decrement 
` -- ` operator

```JS
let decrement = 0;

decrement--;
console.log(decrement)  ----->  -1

decrement--;
console.log(decrement)  ----->  -2
```

Applies in the same way as increment


## Exponential
` ** ` operator

```JS
console.log(5 ** 2)  ----->  25
```