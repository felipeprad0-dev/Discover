# Scope let 

    * Let variables are local scope only works inside block where it was created 
    * Let must be declared at the beginning of the code, before any statement
    * Your value can be reassigned within the block that the variable belongs to

---------------
    console.log("is there a variable y before the block?", y)     ------>    if we execute this code, the result will be: `ERROR`

{
    console.log("is there a variable y inside the block?", y)
    let y = 0;                                                    ------>    if we execute this code, the result will be: `ERROR`
}

{
    let y = 0;
    console.log("is there a variable y inside the block?", y)     ------>    if we execute this code, the result will be: `0`
}

    console.log("is there a variable y after the block?", y)      ------>    if we execute this code, the result will be: `ERROR`
--------------


OR


---------------
    let y = 1;
    console.log("is there a variable y before the block?", y)     ------>    if we execute this code, the result will be: `1`

{
    console.log("is there a variable y inside the block?", y)
    let y = 0;                                                    ------>    if we execute this code, the result will be: `ERROR`
}

{
    let y = 0;
    console.log("is there a variable y inside the block?", y)     ------>    if we execute this code, the result will be: `0`
}

    console.log("is there a variable y after the blocks?", y)      ------>    if we execute this code, the result will be: `1`
--------------



OR



---------------
    let y = 1;
    console.log("is there a variable y before the block?", y)     ------>    if we execute this code, the result will be: `1`

{
    console.log("is there a variable y inside the block?", y)
    y = 0;                                                    ------>    if we execute this code, the result will be: `ERROR`
}

{
    y = 0;
    console.log("is there a variable y inside the block?", y)     ------>    if we execute this code, the result will be: `1`
}

    console.log("is there a variable y after the blocks?", y)      ------>    if we execute this code, the result will be: `1`
--------------
