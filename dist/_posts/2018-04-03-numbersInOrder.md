---
Post:   
Title:  "numbers In Order"
Date:   2018-03-09
Categories: ""

---
# numbers In Order 

## Introduction 
I toke one of my code kata's that i did on Codewars and decided to refactor my code and make it more cleaner using ECMAScript arrow function , and giving my variables proper naming.    

### Example 1 
`

function inAscOrder(arr) {
    var originalArray = [];
    for(var i in arr){
        originalArray.push(arr[i]);
    }
     var ascendingOrder = arr.sort(function (a, b) {
        return a - b;
    });
    if (originalArray.join('') === ascendingOrder.join('')) {
        return true;
    } else {
        return false;
    }

};

`
#### Example 2

`
function inAscOrder(array) {  
    var originalArray = [];
    array.forEach((element) => originalArray.push(element));
    var ascendingOrder = array.sort((a, b) => a - b);
    return  originalArray.join('') === ascendingOrder.join('')? true: false;
};

`

If you were to look at the two explains above Example 1 and Example 2 , both functions can accomplishes the same task. But both functions are not written in the
same way .The first Example is a function that has a for loop pushing all the elements into a empty array called originalArray followed by a method called ascendingOrder which sorts the arr
 in ascendingOrder followed by a if else which returns true or false value. depending on the condition. The code is also longer then Example 2 and also just by looking at it you can clearly see
 that is less cleaning then Example 2 . Example 2 is more readable to a point that you can go though it and understand what the code is doing much quicker then the one above Example 1 . 

## So whats the trick ?

the trick is to give your variables proper naming for example i named my function argument array instead of arr , used ECMAScript 6 arrow function to write a forEach instead of a for loop
that allowed me to loop through each element and push it into an empty array all of that in one line. Same with the ascendingOrder i used ECMAScript 6 arrow function to sort and return an array with values in ascendingOrder all of that was accomplished in one line. Ended off by returning a ternary operator in my return statement that returns a boolean true or false.  


## Conclusion 

By writing clean code it makes it a lot easier to example to someone what your code is doing  .Also when your code is clean and readable you don't need to write comments .
One of the ways you can write clean and readable code is by using ECMAScript 6 arrow Functions .You can also use functional programming as a tool to write clean code.   










