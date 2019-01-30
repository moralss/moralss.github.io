---
Post:   
Title:  "droping elements in the array"
Date:   2018-03-13
Categories: ""

---
# Droping elements in the array

## Introduction 
The reason why i choice to wrote a blog post about this , was because of the level of difficulty i in counted when solving this challenge a challenge i got from FreeCodeCamp.


## Instructions 

Drop the elements of an array (first argument), starting from the front, until the predicate (second argument) returns true.

The second argument, func, is a function you'll use to test the first elements of the array to decide if you should drop it or not.

Return the rest of the array, otherwise return an empty array.



## Solution 
### Code
`
function dropElements(arr, func) {
  
  while(!func(arr[0])){
      arr.shift();
  }
  return arr;
}

console.log(dropElements([1, 2, 3], function(n) {return n < 3; }));

`

Solving this Challenge i first started by using the filter function which is a built in function in Javascript which filters according to the conditions you set for the arguments . I used this function but passed in function called func
but it was giving me all the elements which was less the the condition and basically returning me the wrong results.  it toke me some time but i managed to figure out another way  ,
 using a while loop and checking the first index of the arr if it passes the condition and if not i removed the element out of the array .


## Conclusion 
leant about the shift() function which helped me solve this challenge.