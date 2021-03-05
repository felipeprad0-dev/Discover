# New

_Left-hand-side expression. It's used to create an object._

Example:

```JS 

let name = new String('Felipe')
let age = new Number(25)

console.log(name, age)      ----->      String {"Felipe"}
                                        Number {25}

name.surName = "Prado"

console.log(name)           ----->      Stringb {"Felipe", surName: "Prado"}
```