# Logical Operators

_Two boolean values that when checked, will return true or false._


## Signals 

` && `       ----->       And 

` || `       ----->       Or 

` ! `        ----->       Not


## AND ` && `

```JS
let bread = true 
let cheese = true 

console.log(bread && cheese)      ----->      true
```

```JS
let bread = false 
let cheese = true 

console.log(bread && cheese)      ----->      false
```

```JS
let bread = true 
let cheese = false

console.log(bread && cheese)      ----->      false
```

```JS
let bread = false 
let cheese = false

console.log(bread && cheese)      ----->      false
```



## OR ` || `

```JS
let bread = true 
let cheese = true 

console.log(bread || cheese)      ----->      true
```

```JS
let bread = true 
let cheese = false 

console.log(bread || cheese)      ----->      true
```

```JS
let bread = false 
let cheese = true 

console.log(bread || cheese)      ----->      true
```

```JS
let bread = false 
let cheese = false 

console.log(bread || cheese)      ----->      false
```



## NOT ` ! `

```JS
let bread = true 
let cheese = true 

console.log(!bread)         ----->      false
console.log(!cheese)      ----->      false
```

```JS
let bread = true 
let cheese = false 

console.log(!bread)         ----->      false
console.log(!cheese)      ----->      true
```

```JS
let bread = false 
let cheese = true 

console.log(!bread)         ----->      true
console.log(!cheese)      ----->      false
```

```JS
let bread = false 
let cheese = false 

console.log(!bread)         ----->      true
console.log(!cheese)      ----->      true
```