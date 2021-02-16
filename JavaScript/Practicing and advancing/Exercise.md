1. Declare a variable named weight:

    var weight;

------------------------------------------------------------------------------------------------------------------------------------------------------

2. What is the data typo of the variable above?

    Undefined ---> console.log(typeof weight)

------------------------------------------------------------------------------------------------------------------------------------------------------

3. Declare a variable and assign values to each of the data: 
    * name: String
    * age: Number (Integer)
    * weight: Number (Float)
    * isSubscribed: Boolean 


    var name = "Felipe"
    var age = 25
    var weight = 105.8
    var isSubscribed = false

------------------------------------------------------------------------------------------------------------------------------------------------------

4. What is the data type of the student variable below?

    var student = {}

    It's an Object.


    4.1. Assign to it the same properties and values of the exercise 3: 
    4.2. Show the following message on the console: 

        <name> is <age> years old and he weighs <weight> Kg.

        Look out, change <name> <age> and <weight> values to object property values

    var student = {
        name: "Felipe",
        age: 25,
        weight: 105.8,
        isSubscribed: false
    }

    console.log("${student.name} is ${student.age} years old and he weighs ${weight} Kg.)

------------------------------------------------------------------------------------------------------------------------------------------------------
    
5. Declare a variable as an array type, named students and assign it no value, that is, only the empty array:

    var students = [];

------------------------------------------------------------------------------------------------------------------------------------------------------

6. Reassign the value to the variable above, putting the student object of question 4 inside it:

    students = [
        student
    ]

------------------------------------------------------------------------------------------------------------------------------------------------------

7. Put the zero index value of the above array on the console: 

    console.log(students[0]);

------------------------------------------------------------------------------------------------------------------------------------------------------

8. Create a new student and put it in the index 0 of the Students Array:

    const john = {
        name: "John",
        age: 20,
        weight: 80.0,
        isSubscribed: true
    }

    Reassigning: 
    students = [
        student,
        john
    ]


    Adding: 
    students[1] = john

    
    With the splice function
    var students = [ student ]

    students.splice(index, number to be removed after the left index, item)
    students.splice(1, 0, john);

------------------------------------------------------------------------------------------------------------------------------------------------------

9. What is the answer of the code below and why? After answering, run the code and check if it works.

    console.log(a)
    var a = 1;  

    The answer will be `Undefined`!!!