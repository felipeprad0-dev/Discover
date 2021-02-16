# Arrays

## Empty Array 

    const animals = []


## Array with Elements 

    const animals = [
        'Lion',
        'Monkey',
        'Cat'
    ]

## Array Indexes 

    The position of the indexes in the arrays starts at 0
    Example: 



                    Item 1    Item 2   Item 3 
                       |        |        |
                       |        |        | 
    const animals = ['Lion', 'Monkey', 'Cat']  
                       |        |        |
                       |        |        |
                    Index 0  Index 1  Index 2


## Show the Total Elements of an Array

    console.log(animals.length) ------> 3


## Show all the Elements of an Array

    console.log(animals) ------> (3) ["Lion", "Monkey", "Cat"]

## Access an Element of an Array

    console.log(animals[Index])
    console.log(animals[0]) ------> Lion 
    console.log(animals[1]) ------> Monkey 
    console.log(animals[2]) ------> Cat 


## Access the Last Element of an Array 

    console.log(animals[animals.length - 1]) ------> Cat

## Add an Item to the beginning of an Array

    var addBeginning = animals.unshift('Dog') ------> (4) ["Dog", "Lion", "Monkey", "Cat"]

## Add an Item to the End of an Array

    var addEnd = animals.push('Horse');

    console.log(animals) ------> (5) ["Dog", "Lion", "Monkey", "Cat", "Horse"]

## Remove the First Item of an Array 

    var removeFirst = animals.shift() ------> (4) ["Lion", "Monkey", "Cat", "Horse"]


## Remove the Last Item of an Array

    var removeLast = animals.pop() ------> (3) ["Lion", "Monkey", "Cat"]


## Search the Index of an Item

    var position = animals.indexOf('Monkey') ------> 1


## Remove an Item by Index Position

    var removedItem = animals.splice(pos, 2) ------> (2) ["Lion", "Monkey"]


## Remove Items of a Index Position 

    const animals = ["Lion", "Monkey", "Cat", "Horse"]

    var pos = 1, n = 2;

    var removedItems = animals.splice(pos, n);

    console.log(animals) ------> (2) ["Lion", "Horse"]

    console.log(removedItens) ------> ["Monkey", "Cat"]


## Copy an Array 

    var copy = animals.slice()


## Array with an Object 

    const animals = [
        'Lion',
        'Monkey',
        [
            name: 'Cat',
            age: 3
        ]
    ]

## Access the Object Inside an Array 

    console.log(animals[1].name) ------> Undefined (because there isn`t a object in the index 1)

    console.log(animals[2].name) ------> Cat