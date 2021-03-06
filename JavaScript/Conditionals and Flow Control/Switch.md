# Switch

_To `switch` statement is used to perform different actions based on different conditions._

_We have to use the `break` at the end because to stop the execution._


## Syntax
```JS
switch(expression) {
    case x: 
        // code block
        break;

    case y: 
        // code block
        break;

    case z:
        // code block 
        break;
}
```


## Examples 
```JS
let expression = 'a'

switch (expression) {
    case 'a': 
        console.log('a');
        break;

    case 'b': 
        console.log('b');
        break;

    default:
        console.log('default'); 
        break;
}
```


## Calculator 
```JS
function calculate(number1, operator, number2) {
    let result;

    switch(operator) {
        case '+':
            result = number1 + number2;
            break;

        case '-':
            result = number1 - number2;
            break;

        case '*':
            result = number1 * number2;
            break;

        case '/':
            result = number1 / number2;
            break;

        default:
            console.log('Not implemented');
            break;
    }

    return result;
}
```