---
Post:
Title:  "progress"
Date:   2018-02-15
Categories:

---
# Finding longest string 

## introduction

 Finding the longest word in a string was a challenge that i got form FreeCodeCamp.

 ## instruction 
Return the length of the longest word in the provided sentence.

Your response should be a number.


## solution 

         function findLongestWord(string) {

            var longestWord = "";

            var changeIntoAnArray = string.split(' ');


            var sortArray = changeIntoAnArray.sort(function (a, b) { return b.length - a.length; });
            
            longestWord = sortArray[0];

            return longestWord.length;

}

When i was writing the algorithm i decided to take the string that was passed in as an argument and convert it into an array. What i battled with the most was sorting the array by the length of the words in the array. So i searched it up on StackOverFlow . After getting a way to sort the array , i them returned the first element in the array.

## conclusion 



### reference 

https://stackoverflow.com/questions/10630766/sort-an-array-based-on-the-length-of-each-element

