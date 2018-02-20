---
Post:
Title:  "progress"
Date:   2018-02-14
Categories:

---
# Capitaling every letter in a string 


## introduction
 
creating a function that returns the first letter of of every string capitalized. This challenge was given to me on FreeCodeCamp. 

## instructions

Return the provided string with the first letter of each word capitalized. Make sure the rest of the word is in lower case.

## solution

var emptyArray = [];

function capitalizeFirstLetters(stringToBecapitalized) {
    stringToBecapitalized = stringToBecapitalized.toLowerCase();
    var turnStringIntoArray = stringToBecapitalized.split(' ');

    for (var i = 0; i < turnStringIntoArray.length; i++) {

        var firstIndexOfEveryWord = turnStringIntoArray[i][0];

        var firstIndexCapitalize = firstIndexOfEveryWord.toUpperCase();

        replaceFirstIndexOfEveryWord = turnStringIntoArray[i].replace(firstIndexOfEveryWord, firstIndexCapitalize);
        emptyArray.push(replaceFirstIndexOfEveryWord);

        

    }
    return emptyArray.join(' ');
}

I created a function called capitalizeFirstLetters , which passed in a string . I set the initial string to became lower case letters 
, converted the string to became a array which i looped though founding the first index of every word and capitalizing it .I added the capitalized string into a new array called empty array which i turned back into a string with the join() function. 


## conclusion 


At first i battled to get this right due to the fact that i did not know build in functions for Javascript . so i did some research on 
W3school to get and understanding on how and what the different Javascript function are. And thats how i managed to complete this challenge on FreeCodeCamp. 








