# Arrow Function 

_italic Arrow function is a modern way to declare functions. This method doesn`t accept hoisting._ 

```JS 

const sayMyName = () => {
    console.log('Felipe');
}

sayMyName()         ---------------> Felipe

```


```JS 

const sayMyName = (name) => {
    console.log(name);
}

sayMyName()    -----------------> Undefined

```

```JS 

const sayMyName = (name) => {
    console.log(name);
}

sayMyName('Felipe')    -----------------> Felipe

```