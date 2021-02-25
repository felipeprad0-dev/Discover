# Functions 

    The functions are one of the fundamentals building blocks in JavaScript.
    A Function in JavaScript is similar to procedure, a set of statements thats performes a task or calculates a value.
    Use functions to facilitate the code, so we don't have to repeat some statements. 


## Function Declarations

    A function definition (also called function declaration, or function statement), consist of the function keyword, followed by: 

        - The name of the function. 
        - Parameters to the function, enclosed in parentheses and separated by commas.
        - The statements that define the function, enclosed in curly brackets. 

    Example: 

            function functionName(parameters) {
                declaration;
            }


            function seeSomething() {
                console.log("Something");
            }

                          
            function square(number) {
                return number * number;
            }


## Execute / run / call / invoke

    To execute the function, we just have write the function name, followed by parentheses.

    function seeSomething() {
        console.log("Something");
    }

    seeSomething();