# Swift: Brief Introduction

### Purpose (5 Mins)
The purpose of the introduction is to let the learners be aware that there is a new native ios coding language called swift that is used to not only create apps for mobile devices but also for macOS, watchOS, tvOS app. Many parts of swift are similar to Objective-C, but is easier to read and also contains all the basic data types. The most recent version of Swift currently is 5.0

### Learning Objectives
By the end of the day learners will be able to:
1. Know how to create variables and constants
1. Know how to use simple data types
1. Know how to use arrays and loops
1. Know how to use IDE XCode
1. Know the process in how to create a 'Hello World' App


### Setup (5 Mins)
The purpose here to to make sure everyone has XCode or a version of it running on their machines. Emphasize that XCode is not supported on Windows based machines and is strictly for those that own machines that run a MacOS operating system.

Have users do the following before diving into the code to make sure they are all setup to play around with the code as they feel comfortable afterwards.
1. Open XCode
1. Click on ```Get started with playground```
1. Click on ```Blank``` under the iOS tab and click ```next```
1. Give the playground a name like you would any file and select where to store it on your machine before clicking ```Create```

Now that users have a blank playground to work with and experiment code with, show them that the boilderplate code or any code you put into the editor can be ran line by line and the results will display on the right hand side console. The console on the bottom is the error log.

Everyone should see something like this.. [Insert Screenshot Link Here](www.google.com).

## Syntax (45 mins)

### Data Types and Operators
#### Instructor-Do
Show learners that swift contains the basic data types of ```Int, Bool, String, Character``` and the basic operators such as ```+, -, =, +=, -=```. Make a note that you cannot apply basic operators to data tyes such as Bool. As you go through the operatos line by line in playground, purposefully show that if the indentations between the left-side variable and operator are not the same as the right-side variable and the operator, that it will cause a syntax error (ie, var intVal+= 3) it should be ```var intVal += 3```, point out how both sides have even spacing between the operator!

### Variables and Constants
By now, learners should have noticed the that for the syntax we are using, its been a keyword of var, then the name of the variable and then an operator that we are assigning it to. The ```var``` keyword allows us to declare a variable and then Swift will automatically infer the data type associated with the declaration as such.
```
var greeting = "Hello!"
greeting = "Bye!"
```
As with any programming language, you cannot set the variable to another type after it has been declared, you either need to create a new one and convert from the already existing one. There is another keyword ```let``` that creates a constant. These cannot be modified after they are created and you can show that in playground by trying to set the constant to a different variable after and you will get an error.
```
const greeting = "Hello!"
greeting = "set to something else!"
``` 
#### Instructor-Do
Show leaners how to create variables and constants in playground.


### Explict Declaration
You can also define variables and their types explicitly in Swift. It is an OOP language in that you can create classes to use later and this is where defining variables types comes in handy. To do so, you can define it like such: ```var intVal: Int()``` and that is the equivalent of saying ```var intVal = 0```. Intial values will be nil or nothing at first (Note: nil can be thought of as null for those that come from coding backgrounds) so you can assign values after declaring it or do it all in one step like ```var intValue: Int = 33```. All 3 are perfectly valid here, and the more you use the language, the more familiar you will become in knowing when you use which form and where.
#### Instructor-Do
Show learners how to explictly declare a variable in playground.


#### You-Do
Have learners create each data type in their playground and then call up a few to walk the instructor in the syntax used to create them. BONUS: Have them create the types with the 3 different forms they can use. 

### Collections and Loops
Swift has 3 major collections that are offered: Arrays, Sets, and Dictionary. We will focus on Arrays for now until Sets and Dictionary come into the picture. Arrays have an index and a value associated with that index. You can only hold one data type in any declared array, but we can create an object of arrays that can contain many different properties of different types. Declaring an array in Swift goes as follows: ```var myArray = [String]```. This creates an array that takes in String types. You can set values of the array by declaring the name of the array and then the index that you want to set like so: ```myArray[2] = "Mary"```. Remember that we can declare and set the values all in one step like so: ```var myArray: [String] = ["Mary", "Had", "A", "Little", "Lamb"] ```.
#### Instructor-Do
Show learners how to create an array in playground.

### You-Do
Have learners create arrays of 2 types and have them set 3 values in each. BONUS: Create the arrays in one step.

### Loops
Loops are essentially in the form of for-each in swift. You need to create a local variable to iterate through the variable of the collection ie an array as such
```
let myArray = ["Mary", "Had", "A", "Little"]
for words in myArray {
    print("Hello, \(word)!")
}
``` 
Point out that the 'words' word is a local variable that is used to contain one element of the array at any given time. Make note of the print statement as well - the syntax for using a variable in a print statement must be done through a a string literal using ```\({name of variable})``` We haven't had to use the print statement much in playground because the console prints everything line by line, but in an actual environment where we are working on a project, we will not have that will have to rely on print to get specific values. You can also iterate through a specific index ie
```
for index in 1...5 {
    print("\(index) times 5 is \(index * 5)")
}
```
This syntax is just saying to take numerical values from 1 all the way to 5 (inclusive) and then do logic within the loop, and in this case, we are just printing.

#### We-Do
Go through with the learners how to iterate through an array with a collection like an array and then with just indexes.

## Break

## Creating our first iOS Hello World App (45 mins)



