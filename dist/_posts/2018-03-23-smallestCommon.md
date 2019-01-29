---
Layout:	
Title:	"smallest Common Multiple"
Date:	2018-03-20 
---

# smallest Common Multiple

## Introduction 

solving a Math problem finding the Lowest Common Multiple.

## instructions 

Find the smallest common multiple of the provided parameters that can be evenly divided by both, as well as by all sequential numbers in the range between these parameters. The range will be an array of two numbers that will not necessarily be in numerical order.
e.g. for 1 and 3 - find the smallest common multiple of both 1 and 3 that is evenly divisible by all numbers between 1 and 3.

## Solution 
### code
`

function smallestCommons(arr) {
  
  var maxRange = Math.max(arr[0], arr[1]);
  var minRange = Math.min(arr[0], arr[1]);

  var lcm = 0;
  var flag = true;
  
  while (flag) {
    lcm++;
    for (var i = minRange; i <= maxRange ; i++) {
      if (lcm % i !== 0) {
        break;
      }

      if (i === maxRange) {
        flag = false;
      }
    }
  }
  return lcm;

}
`

I started by creating a function called smallestCommons which toke in an array called arr that contained two element values in the array, for example, it could contain  [1,5] or [5,1]. I then created a variable called maxRange which determined the maximum value 
between the two elements and another variable called minRange which contained the minimum value between the two values in the array.
I Then created a variable called lcm and i set it to 0 and a flag which stores a boolean and i set it to true.
After setting my variables i then used a while loop to loop until the flag was false incrementing lcm. Followed by a for loop which loops form a starting position of minRange to the maxRange. Inside the for loop I wrote a conditional statement which checks if each value for Modulus meaning for each time there is a reminder when lcm is divided by i ,then break the for loop and increment lcm and if  i is equal to maxRange then flag is equal to false and the while loop stops the a value called lcm is returned.


## conclusion 

This is the method i used to solve the smallest Common Multiply,a challenge i got on FreeCodeCamp. this solution might not be 
the best, but its definitely my solution and it works for me.


