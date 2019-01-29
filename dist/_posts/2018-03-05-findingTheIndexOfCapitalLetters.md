---
Post:
Title:  "finding the index of all the capital letters"
Date:   2018-03-05
Categories:

# CodeWars  

## Introduction 

The kata i did on CodeWars helping me understand a few things to do with validating a password checking if a password consist of certain  criterias. Like does it consist of enough captial letters
.

## Instructions
I had to create a function that had to find the index of all the capital letters in a string and return them in an array.



## solution 

i got the index by first splitting the string making it into an array , so that i cant loop through it and identify all the captial letters . the results i then pushed them to an empty array and return 
the empty array with all the capital letters.

`

var capitals = function (word) {

    var splitted = word.split('');
    var res = [];
    for (var i in splitted){
        if(splitted[i] === splitted[i].toUpperCase()){
            res.push(splitted.indexOf(splitted[i]));
        }
    }
    return res;
};

console.log(capitals("HellO"));

`


## Conclusion 


Had so much fun with the kata that i did on CodeWars .