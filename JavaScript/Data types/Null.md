# Null 

    * Nulo 
    * Objeto que não possui nada dentro 
    * Diferente de indefinido 

typeof x             // 'undefined'
typeof y             // 'object'


var x;

x == null            // true
x == undefined       // true
x === null           // false
x === undefined      // true (x não tem valor!)

var y = null;

y == null            // true
y == undefined       // true
y === null           // true
y === undefined      // false (y existe, e seu valor é null)