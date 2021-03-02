# Manipulating Arrays

let techs = ["html", "css", "js"]


## Adding an item to the end
```JS
techs.push("nodejs")
console.log(techs)       ----->       (4) ["html", "css", "js", "nodejs"]        
```


## Adding an item to the beginning
```JS
techs.unshift("SQL")
console.log(techs)       ----->       (5) ["SQL", "html", "css", "js", "nodejs"] 
```


## Removing an item from the end 
```JS
techs.pop()
console.log(techs)       ----->       (4) ["SQL", "html", "css", "js"] 
```


## Removing an item from the beginning
```JS
techs.shift()
console.log(techs)       ----->       (3) ["html", "css", "js"] 
```


## Picking only a few elements from the array 
_This method receive as an argument the initial index and the array length. ---> `.slice(initialIndex, Arraylength)`_
```JS
console.log(techs.slice(1,3))       ----->       (2) ["css", "js"] 
```


## Removing one or more items from the array
_This method receive as an argument the index of the element and the number of elements we want to remove (after the initial index). ----> `.splice(indexOfTheElement, numberOfElements)`_
```JS
console.log(techs.splice(1,1))       ----->       (2) ["css"] 
```

if we want to take off two elements, 

```JS 
console.log(techs.splice(1,2))       ----->       (5) ["SQL", "js", "nodejs"]
```


## Find the position of an element in the array
```JS

let techs = ["SQL", "html", "css", "js", "nodejs"]

console.log(techs.indexOf('css'))       ----->     2   
```

or 


```JS 
let techs = ["SQL", "html", "css", "js", "nodejs"]

let index = techs.indexOf('css')

console.log(index)      ------->       2
```

and removing 
```JS
tech.splice(index, 1)