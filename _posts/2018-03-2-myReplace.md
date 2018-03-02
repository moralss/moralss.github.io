---
Post:
Title:  "local Weather Machine"
Date:   2018-02-16
Categories:

# freeCodeCampChallenges  

## Introduction 



## Instructions

Perform a search and replace on the sentence using the arguments provided and return the new sentence.

First argument is the sentence to perform the search and replace on.

Second argument is the word that you will be replacing (before).

Third argument is what you will be replacing the second argument with (after).

NOTE: Preserve the case of the original word when you are replacing it. For example if you mean to replace the word "Book" with the word "dog", it should be replaced as "Dog"

## solution 
`
function myReplace(str, before, after) {

    var ConvertSTringIntoArray = str.split(' ');
     var index =  ConvertSTringIntoArray.indexOf(before);
     
    var beforeFirstIndex = before.charAt(0);
    var beforeCapitalizedIndex = before.charAt(0).toUpperCase();




    if (beforeFirstIndex === beforeCapitalizedIndex) {

        ConvertSTringIntoArray[index] = after.charAt(0).toUpperCase() + after.slice(1);

        finalString = ConvertSTringIntoArray.join(' ');
        
    }

    else{

         ConvertSTringIntoArray[index] = after;

        var finalString = ConvertSTringIntoArray.join(' ');
    }

    return finalString;
};

console.log(myReplace("A quick brown fox jumped over the lazy dog", "jumped", "leaped"));
console.log(myReplace("He is Sleeping on the couch", "Sleeping","sitting"));


`

i started by creating my global variables , a variable to convert my string into an array , one for determining the position of the index of the string that had to be changed . The other two was to get the first index of the string passed in as a perimeter Before. 

 i then wrote a if statement to determine if the perimeter Before had a first index which consisted of a captial letter or not .Replaced the second perimeter Called Before with the third perimeter called After, which then changed the text;   


## Conclusion 


leant about charAt . had so much fun           

