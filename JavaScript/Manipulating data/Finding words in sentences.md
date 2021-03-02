# Find Words in Sentences

_Use the `.includes()` method._

_This method is case sensitive, so we have to put exactly the same word!_


## Checking if the word "Love" exists 

```JS

let phrase = "I wanna live!";

console.log(phrase.include("Love"))     ----->      false, because there is no word love.

```



```JS 

let phrase = "I wanna live the love";

console.log(phrase.include("Love"))     ----->      false, there is the word love, but the method is casesensitive, so it is different.

```



```JS

let phrase = "I wanna live the Love";

console.log(phrase.include("Love"))     ----->      true

```