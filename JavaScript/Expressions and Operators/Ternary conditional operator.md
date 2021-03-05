# Ternary Conditional Operator

_Depending of the condition, we will receive different values._

_Condition `so` value 1 `if not` value 2_
_Condition `?` value 1 `:` value 2_





## Examples With Breakfast

## Breakfast with AND ` && `
```JS
let bread = true
let cheese = true

const niceBreakfast = bread && cheese ? 'Nice breakfast' : 'Bad breakfast'

console.log(niceBreakfast)      ----->      'Nice breakfast'
```

```JS
let bread = false
let cheese = true

const niceBreakfast = bread && cheese ? 'Nice breakfast' : 'Bad breakfast'

console.log(niceBreakfast)      ----->      'Bad breakfast'
```

```JS
let bread = true
let cheese = false

const niceBreakfast = bread && cheese ? 'Nice breakfast' : 'Bad breakfast'

console.log(niceBreakfast)      ----->      'Bad breakfast'
```

```JS
let bread = false
let cheese = false

const niceBreakfast = bread && cheese ? 'Nice breakfast' : 'Bad breakfast'

console.log(niceBreakfast)      ----->      'Bad breakfast'
```



## Breakfast with OR ` || `
```JS
let bread = true
let cheese = true

const niceBreakfast = bread || cheese ? 'Nice breakfast' : 'Bad breakfast'

console.log(niceBreakfast)      ----->      'Nice breakfast'
```

```JS
let bread = false
let cheese = true

const niceBreakfast = bread || cheese ? 'Nice breakfast' : 'Bad breakfast'

console.log(niceBreakfast)      ----->      'Nice breakfast'
```

```JS
let bread = true
let cheese = false

const niceBreakfast = bread || cheese ? 'Nice breakfast' : 'Bad breakfast'

console.log(niceBreakfast)      ----->      'Nice breakfast'
```

```JS
let bread = false
let cheese = false

const niceBreakfast = bread || cheese ? 'Nice breakfast' : 'Bad breakfast'

console.log(niceBreakfast)      ----->      'Bad breakfast'
```





### Examples With Age

## Age with GREATER THAN or EQUAL TO ` >= `
```JS
let age = 16

const canDrive = age >= 18 ? "Can drive" : "Can't drive"

console.log(canDrive)      ----->      "Can't drive"
```


## Age with LESS THAN or EQUAL TO ` <= `
```JS
let age = 18

const canPlay = age <= 16 ? "Can play" : "Can't play"

console.log(canPlay)      ----->      "Can't play"
```


## Age with EQUAL TO ` == `
```JS
let age = 25

const canComeIn = age == 25 ? "Can come in" : "Can't come in"

console.log(canComeIn)      ----->      "Can come in"
```



