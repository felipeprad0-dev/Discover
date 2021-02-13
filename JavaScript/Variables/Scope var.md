# Scope var 
    
    * Var variables are global scope and can work inside and outside of a block
    * Your value can be reassigned across the entire scope

---------------
    console.log("is there a variable x before the block?", x)     ------>    if we execute this code, the result will be: `undefined` , because the `hoisting behaviour`

{
    var x = 0;                                                    ------>    if we execute this code, the result will be: `0`
}

    console.log("is there a variable x after the block?", x)      ------>    if we execute this code, the result will be: `0`
--------------
