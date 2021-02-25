# Constructor Functions 
_It's basically a function and can be explained as a model, a structure that describes states and behaviors of an object. It can be executed as a function or to be used to instantiate an object, using the reserved word `new`._

_It's a good practice to declare the name of the construction function with the capital letter._ 


## New operator 
_New operator is used to create (instance) an object._ 


## This keyword 
_This keyword is used to reference the created object._


```JS

function Person(name, age, city) {
    this.name = name;
    this.age = age;
    this.city = city;
}

const felipe = new Person('Felipe', 25, 'Sao Simao')

console.log(felipe);

```


_-------------------------------ANOTHER CASE-------------------------------_


```JS 

function Person(name, age, city) {
    this.name = name;
    this.age = age;
    this.city = city;
}

const felipe = new Person();
felipe.name = 'Felipe';
felipe.age = 25;
felipe.city = 'Sao Simao';

console.log(felipe);

```

