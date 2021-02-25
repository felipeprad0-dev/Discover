# Function Hoisting 

_italic Hoisting is JavaScript's default behavior of moving declarations to the top of the current scope (to the top of the current scope or the current function)_

_italic When we try to run a function by declaring it later, this function will receive the `hoisting behavior` and run normally. But, when we try to run a function that is storaged within a variable, it will return an error!_


```JS 

sayMyName();

function sayMyName() {
    console.log("Felipe");          -------> Felipe
}

```


```JS 

sayMyName();

const sayMyName = function() {
    console.log("Felipe");          -------> Uncaught ReferenceError: Cannot access 'sayMyName' before initialization
}

```

