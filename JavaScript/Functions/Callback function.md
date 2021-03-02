# Callback Function

_Callback is a function declared as parameter for another function. Callbacks are declared as functions to be executed after a certain event. It will be wait for something happen to act (run)._

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


_-------------------------- ANOTHER CASE --------------------------_

```JS

function callback(e) {
    alert('An event happened' + e.type);
}

window.addEventListener('click', callback);

```
