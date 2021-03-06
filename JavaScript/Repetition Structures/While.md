# While

_The `while` statement creates a loop that executes a specified statement as long as the test condition evaluates to true. The condition is evaluated before executing the statement._


# Syntax

while (condition) {
    statement
}


## Example infinity while 

_In this case, we dind't declare an update to `i`, the loop will be infinity._

```JS
let i = 0;

while (i < 10) {
    console.log(i);             ------>         Infinity
}
```


## Example updating the variable value 

_In this case, we declare the `i++` to update the variable value, then it will not be an infinity loop._

```JS
let i = 0;

while (i < 10) {
    console.log(i);             ------>         0, 1, 2, 3, 4, 5, 6, 7, 8, 9
    i++;
}
```


## Example with end that we don't know

_In this case, we declare the `i /= ` to divide the variable value, and as long as the result is greater than 10, the loop will not stop._
_The loop stopped at `28.651593787022893` because the next number would be less than 10._ 

```JS
let i = 64519818951181;

while (i > 10) {
    console.log(i);              ------>    64519818951181, 1843423398605.1714, 52669239960.14775,
                                            1504835427.432793, 42995297.926651224, 1228437.0836186064,
                                            35098.20238910304, 1002.8057825458012, 28.651593787022893             
    i /= 35;
}
  