# Throw 

_This statement throws an user-defined expression. Execution of the current function will stop (the statements after throw won't be executed), and control will be passed to the first catch block in the call stack. If no catch block exists among caller functions, the program will terminate._


# Try...Catch

_The try...catch statement marks a block of statements to try and specifies a response should an exception be thrown._




## Example with no Try...Catch

_In this case, the name has not been defined, then the application will break and will not perform anything else._

```JS
function sayMyName(name) {
    if (name === undefined) {
        throw new Error('Name is required!');
    }

    console.log('Error');           ----> It will not be executed
}

sayMyName();

console.log('Continue')         ----> It will not be executed

// try {
//     sayMyName();
// } catch(e) {
//     console.log(e);
// }
```




## Example with Try...Catch

_In this case, the name has not been defined but there is the try...catch, then the application will break, the catch will capture the error and the application will continue to work._

```JS
function sayMyName(name) {
    if (name === undefined) {
        throw new Error('Name is required!');
    }

    console.log('Error');           ----> It will not be executed
}

try {
    sayMyName();
} catch(e) {
    console.log(e);
}

console.log('After the error')      ----> It will be executed and show the message 
```




## Valid example with Try...Catch

_In this case, the name has been defined and there is the try...catch, then the application will not break and everything will perform well._

```JS
function sayMyName(name) {
    if (name === undefined) {
        throw new Error('Name is required!');
    }

    console.log('Error');           ----> It will be executed and show the message
}

try {
    sayMyName('Felipe');            ----> It will be executed
} catch(e) {
    console.log(e);
}

console.log('After the error')      ----> It will be executed and show the message 
```