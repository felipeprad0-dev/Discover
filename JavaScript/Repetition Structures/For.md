# For

_Use `for` statement creates a loop that consists of three optional expressions, enclosed in parentheses and separated by semicolons, followed by a statement (block statement) to be executed in the loop._

_`break` to stop the loop._

_`continue` to skip the current execution._


# Syntax

for (initialization; condition; final-expression) {
    statement
}


## Examples
```JS
for (let i = 0; i <= 10; i++) {
    console.log(i);             ---------> 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10
}
```


```JS
for (let i = 10; i > 0; i--) {
    console.log(i);             ---------> 10, 9, 8, 7, 6, 5 , 4, 3, 2, 1
}
```


```JS 
for (let i = 0; i <= 10; i++) {
    if (i === 5) {
        break;
    }

    console.log(i);             ---------> 0, 1, 2, 3, 4
}
```


```JS
for (let i = 0; i <= 10; i++) {
    if (i > 5) {
        break;
    }

    console.log(i);             ---------> 0, 1, 2, 3, 4, 5
}
```


```JS
for (let i = 1; i <= 10; i++) {
    if (i > 5) {
        break;
    }

    console.log(i);             ---------> 1, 2, 3, 4, 5
}
```


```JS
for (let i = 0; i <= 10; i++) {
    if (i === 5) {
        continue;
    }

    console.log(i);             ---------> 0, 1, 2, 3, 4, 6, 7, 8, 9, 10
}
```
