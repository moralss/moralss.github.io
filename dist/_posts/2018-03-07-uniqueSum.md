---
Post:   
Title:  "Returning the sum of all the elements in an Array"
Date:   2018-03-07
Categories: ""

---
# Unique Sum

## Introduction 
Choice to write this blog post to remind myself two new things that i learnt will doing this Kata, a Kata that i got on CodeWars. 

## instructions 

I had to create a function that takes in an Array, removing all the duplicates and returning the sum of the entire Array. 

## Solution 
### code

function uniqueSum(list) {
    var emptyArray = [];
    var sum = 0;

    if (list.length === 0){
        sum =  null;
    }

    for (var index = 0; index < list.length; index++) {
        if (emptyArray.indexOf(list[index]) === -1) {
            emptyArray.push(list[index]);

            var sum = emptyArray.reduce(function (a, b) {
                return a + b;
            });
        }
    }
    return sum;
}


var values = [1, 4, 4, 2, 5, 3];

`
 Started by creating the function and called it uniqueSum that toke in a parameter called list , then i created two variables  called emptyArray and sum 
if the length of the list is equal to 0 i returned a null , if the List had actual values then i looped through the List .
Checked if emptyArray contained two values that were the same and if not 
i pushed the numbers into a emptyArray .Used the reduce function to get the sum and returned the sum.    
I    
## conclusion 

I enjoyed solving this problem.    












