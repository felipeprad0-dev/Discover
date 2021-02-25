# Returning values inside a function 

`EVERY` function returns a value! Remember that!
!The execution of a function ends when it finds a `return`

_italic When we declare a function with two parameters and also declare two variables with the same name of the parameters, the variables will rewritten the parameters, because we didn't declare the `return`._ 

_italic On the console, the command `console.log` will results `30` because the function is executed and `undefined` because of the absence of `return`._

    ```JS
    const = function sum(number1, number2) {
            console.log(number1 + number2);
        }

    let number1 = 20;
    let number2 = 10;

    console.log(`the number1 is equal to ${number1}`);   -------> 20
    console.log(`the number2 is equal to ${number2}`);   -------> 10
    console.log(` the sum is ${sum(number1, number2)}`); -------> 30  
                                                         -------> Undefined
    ```

_italic If we declare a variable (even when the name is different from the parameter) to store (number1 + number2) inside the function and set to return the variable, it will be returns 30._

    ```JS
    function sum(number1, number2) {
        console.log(number1 + number2);
        var total = number1 + number2;
        return total;
    }

    let number1 = 20;
    let number2 = 10;

    console.log(`the number1 is equal to ${number1}`);      --------> 20
    console.log(`the number2 is equal to ${number2}`);      --------> 10
    console.log(` the sum is ${sum(number1, number2)}`);    --------> 30
                                                            --------> 30
    ``` 
    


    Another example: 


    ```JS
    function sum(number1, number2) {
        var total = number1 + number2;
        return total;
        console.log(number1 + number2); ---> `it doesn't works`
    }

    let number1 = 20;
    let number2 = 10;

    console.log(`the number1 is equal to ${number1}`);      --------> 20
    console.log(`the number2 is equal to ${number2}`);      --------> 10
    console.log(` the sum is ${sum(number1, number2)}`);    --------> 30
    ``` 