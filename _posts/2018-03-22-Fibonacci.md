---
Post:   
Title:  "sum of Fibonacci"
Date:   2018-03-09
Categories: ""

---
# sum of Fibonacci

## Introduction 
Here is my explanation on how i solved this problem of the sum of all the odd numbers in a fibonacci sequence 
## Instructions 

// Given a positive integer num, return the sum of all odd Fibonacci numbers that are less than or equal to num.

// The first two numbers in the Fibonacci sequence are 1 and 1. Every additional number in the sequence is the sum of the two previous numbers. The first six numbers of the Fibonacci sequence are 1, 1, 2, 3, 5 and 8.

// For example, sumFibs(10) should return 10 because all odd Fibonacci numbers less than 10 are 1, 1, 3, and 5.


## Solution 
### Code
`
function sumFibs(num) {

    var fibArray = [1, 1];

    var getlastValueInArray = () => fibArray[fibArray.length - 1];

    var getSecondLastValueInArray = () => fibArray[fibArray.length - 2];

    while (getlastValueInArray() + getSecondLastValueInArray() <= num) {
        fibArray.push(getlastValueInArray() + getSecondLastValueInArray());
    }

    var filterOdd = fibArray.filter((value) => value % 2 !== 0);

    return filterEven.reduce((a , b) => a + b);
}

console.log(sumFibs(4));

`
The trick is to first know how to generate a fibonacci sequence , understanding the concept before calculating the sum of all the odd numbers in the fibonacci sequence is that what i did i understand the problem before solving it with code. Started by creating a function called getLastValueInArray with get the last value in the fibArray and i created a second function that was almost the first 
as the first function but this one returns the value of the second as value of the fibArray . Then i did a while loop which while continue running an less the first value plus the second value is smaller or equal to the num value , and will this while loop is running i am pushing the results into an array called fibArray. which at the end stores all the fibonacci numbers .Then i had to find a way to get all the odd numbers in that sequence of fibonacci numbers , i accomplished that by using a built in function called filter which filtered all the values that was not a odd number. So i was left with values that were odd numbers in a fibonacci sequences , allowing me to use a other built in function called reduce to get the sum of all the odd numbers in a fibonacci sequence.  


## Conclusion 

fun and exciting , i hope my explanation was helpful and using to understand one method of getting the sum of all the odd numbers in a fibonacci sequence. 









