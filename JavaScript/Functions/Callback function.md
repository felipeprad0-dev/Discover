# Callback Function

_Callback function is when we want to call a function inside another function. We declare a the function with a parameter that will be the name of the callback, so we run the function declaring another function inside._

```JS 

function sayMyName(name) {
    name();
}

sayMyName(
    () => {
        console.log('i am in a callback');
    }
)

```

_In another words_

`name` is `() => { console.log("I'm in a callback");}`

So, to run it: `name()`
