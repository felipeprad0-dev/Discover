# Separating Strings 

_Use the `.split()` method to separate._

_Use the `.join()` method to join._


## Separating a text containing spaces into a new array where each text is a position of the array

```JS

let phrase = "I wanna live the Love";

let myArray = phrases.split(" ");       

console.log(myArray)     ----->      ["I", "wanna", "live", "the", "Love"]


```


## Joining the array in a text and placing underscores in the places of the spaces 

```JS 

let phraseWithUnderscore = myArray.join("_")

console.log(phraseWithUnderscore)     ----->      I_wanna_live_the_Love