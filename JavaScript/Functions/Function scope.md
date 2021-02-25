# Function scope

_italic When we declare let variable with no value, it will be a undefined variable. In this case, first and outside of a function._

    `let subject;`

_italic After this, if we declare a function with a parameter named equal the let variable and returning the value, when we call the function and it be executed, the results will be `undefined` too._

    ``` JS
    let subject; 

    function create(subject) {
        return subject;
    }

    console.log(subject);                   ----> Undefined
    console.log(create(subject));           ----> Undefined
    console.log(subject);                   ----> Undefined
    ```

_italic This is happens because the first variable doesn`t have a value._

_italic But, if we now attribute some value to the variable, results will be the value of the variable._

    ``` JS
    let subject = 1 

    function create(subject) {
        return subject;
    }

    console.log(subject);               ----> 1
    console.log(create(subject));       ----> 1
    console.log(subject);               ----> 1
    ```

_italic Even if we remove the parameter of the function!_

    ``` JS
    let subject = 1 

    function create() {
        return subject;
    }

    console.log(subject);               ----> 1
    console.log(create());              ----> 1
    console.log(subject);               ----> 1
    ```

_italic But, if we declare the subject variable inside the function scope but with other value and no type, we will have as a result, the value declared inside the function, counting that there is the parameter. And, the subject variable declared outside the function, continues to have the same result._

    ``` JS
    let subject = 1 

    function create(subject) {
        subject = 2
        return subject;
    }

    console.log(subject);               ----> 1
    console.log(create(subject));       ----> 2
    console.log(subject);               ----> 1
    ```

_italic Now, if we remove the parameter of the function, the results will be the same as the outside variable. But, when we call the function and it will be executed, the `function hoisting` will happen, and the value of the first variable will be rewritten, now being equal to 2._

    ``` JS
    let subject = 1 

    function create(subject) {
        subject = 2
        return subject;
    }

    console.log(subject);               ----> 1
    console.log(create(subject));       ----> 2
    console.log(subject);               ----> 2
    ```

_italic Everything changes when we set the type of the variable inside de function._ 

    ``` JS
    let subject = 1 

    function create(subject) {
        var subject = 2
        return subject;
    }

    console.log(subject);               ----> 1
    console.log(create(subject));       ----> 2
    console.log(subject);               ----> 1
    ```

_italic Another examples_ 

    ``` JS
    let subject; 

    function create(subject) {
        var subject = 2
        return subject;
    }

    console.log(subject);               ----> Undefined
    console.log(create(subject));       ----> 2
    console.log(subject);               ----> Undefined
    ```

    ``` JS
    let subject;

    function create() {
        var subject = 2
        return subject;
    }

    console.log(subject);   ----> Undefined
    console.log(create());  ----> 2
    console.log(subject);   ----> Undefined
    ```