---
Post:   
Title:  "regex"
Date:   2018-03-14
Categories: ""

---
# count Repeats

## Introduction

The reason why i choice to write a blog post about this kata is because i learnt something new by doing this kata . Its called the count Repeats  
 
## Instructions 
Write a function that returns the count of characters that have to be removed in order to get a string with no consecutive repeats.


## Solution 
### Code
`
function countRepeats(str) {
    var splitString = str.split('');
    var count = 0;

    for (var index = 0; index < splitString.length; index++) {
        if (splitString[index] === splitString[index + 1]) {
            console.log("index", splitString[index], index)
            count++;
        }
    }
    return count;
}



`
I read the instructions over and over again until i understood what was required of me , At first i tried to use two for loops and using the index's to compare first index of the ArrayString with the second index. It did not 
workout i battled to get consecutive repeated terms instead it gave me all the duplicates in the String Array . So i figured out a way to use one for loop and compare the two index's that where next to each other and i got it working.  

## conclusion 

i learnt about using one for loop to compare the first index with the next index something that toke me something to understand and implement in my code. 