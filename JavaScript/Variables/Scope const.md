# Scope const
    
    * Const variables are local scope and only works inside the block where it was created
    * Your value can't be reassigned across the scope
    * We can create a new const variable in another block with the same name and set a different value

---------------
    console.log("is there a variable z before the block?", z)     ------>    if we execute this code, the result will be: `ERROR`

{
    const z = 0;                                                    ------>    if we execute this code, the result will be: `0`
}

    console.log("is there a variable z after the block?", z)      ------>    if we execute this code, the result will be: `ERROR`
--------------



OR 



---------------
    const z = 1;
    console.log("is there a variable z before the block?", z)     ------>    if we execute this code, the result will be: `1`

{
    console.log("is there a variable z inside the block?", z)
    const z = 0;                                                    ------>    if we execute this code, the result will be: `ERROR`
}

{
    const z = 0;
    console.log("is there a variable z inside the block?", z)     ------>    if we execute this code, the result will be: `0`
}

    console.log("is there a variable z after the blocks?", z)      ------>    if we execute this code, the result will be: `1`
--------------