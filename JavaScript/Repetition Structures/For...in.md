# For...in

_The `for...in` statement iterates over all enumerable properties of an object that are keyed by strings (ignoring ones keyed by Symbols), including inherited enumerable properties._


# Syntax 

for (variable in object)
  statement


## Example with an object
```JS
let person = {
    name: 'Felipe',
    age: 25,
    weight: 105
}

for(let property in person) {
    console.log(property)           ---->  name, age, weight
}
```



_Another ways to access the properties_



```JS
let person = {
    name: 'Felipe',
    age: 25,
    weight: 105
}

for(let property in person) {
    console.log(preson.name)           ---->  Felipe
}
```


```JS
let person = {
    name: 'Felipe',
    age: 25,
    weight: 105
}

for(let property in person) {
    console.log(preson["name"])           ---->  Felipe
}
```


```JS
let person = {
    name: 'Felipe',
    age: 25,
    weight: 105
}

for(let property in person) {
    console.log(preson[property])           ---->  Felipe, 25, 105
}
```