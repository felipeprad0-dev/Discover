# If and Else

_If the condition is true, is executed the first instruction. If not, the following instruction that will be executed._


## Syntax
```JS
if (condition) {

} else {

}
```


## Examples

```JS 

let temperature = 36.5;

if (temperature >= 37) {
    console.log("It's a fever!");
} else {
    console.log("It's not a fever!");
}

```


```JS

let temperature = 38;

if (temperature >= 37.5) {
    console.log("It's a high fever!");
} else if (temperature >= 37 &&temperature < 37.5){
    console.log("It's a moderate fever!");
} else {
    console.log("It's healthy!")
}

```


```JS

let temperature = 38;
let highTemperature = temperature >= 37.5;
let moderateTemperature = temperature >= 37 &&temperature < 37.5;

if (highTemperature) {
    console.log("It's a high fever!");
} else if (moderateTemperature){
    console.log("It's a moderate fever!");
} else {
    console.log("It's healthy!")
}
