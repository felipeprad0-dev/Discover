# For...of

_The `for...of` statement creates a loop iterating over iterable objects, including: built-in String, Array, array-like objects (e.g., arguments or NodeList), TypedArray, Map, Set, and user-defined iterables. It invokes a custom iteration hook with statements to be executed for the value of each distinct property of the object._


# Syntax 

for (variable of iterable) {
  statement
}



## Example a variable
```JS
let name = 'Felipe';

for (let char of name) {
    console.log(char);          ----> F, e, l, i, p, e
}
```



## Example with an array
```JS
let names = ['Paulo', 'Pedro', 'Pablo'];

for (let name of names) {
    console.log(name);           ----> Paulo, Pedro, Pablo
}
```


