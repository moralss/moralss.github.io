---
Post:   
Title:  "Finders Keeper"
Date:   2018-03-01
Categories: ""

---
# Finders Keepers


## Introduction 
I refactored the code and decided to write a blog post about it.


## Instructions 

Create a function that looks through an array (first argument) and returns the first element in the array that passes a truth test (second argument).

## Solution 
### Code
`

function findElement(array, functionCondition) {
  
  return array.filter(functionCondition)[0];
     
}

findElement([1, 2, 3, 4] , function(number){ return number % 2 === 0; });


` 

Created a function and gave it a name called findElement which passes in an array and a function as a perimeter. Inside the function i used a concept called Functional Programming .
 One of the methods i used was the filter function
which i then passed in the argument functionCondition . functionCondition is a function by its self which checks if the element in an array is a even number ,if so it returns the first element that is an odd number in an array. 

## Conclusion 
checked the naming of my variables to make it more descriptive. 






