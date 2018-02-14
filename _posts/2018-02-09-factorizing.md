---
Post:   
Title:  "Math"
Date:   2018-02-09
Categories: ""

---
# factoralizing 

## introduction 
Started learning the basics of javascript and moved on to basic Algorithm Scripting.

## instructions 

I had to create a function that returns the factorial of the provided integer , that is passed in as an argument.

## solution 

### code 
var arrNumbersToFactorlize = [];
var sumTotal = 1;

function factorialize(Number) {

    for (var i = 1; i <= Number; i++) {
        arrNumbersToFactorlize.push(i);
    }

    for (var i = 1; i <= arrNumbersToFactorlize.length; i++) {
        sumTotal = sumTotal * i;

    }
    return sumTotal;
}


 

I started off by creating a empty array followed by a variable called sum which stores an integer value of 1. 

Followed by a function that passes in an argument of number. 
I then created an array of all the numbers smaller then the argument number but greater and equal to 1 and  multiplied the values in the array with each other.
To get a sum total which i returned at the end; 


## conclusion 

The exercise was not that hard because i once did this exercise in Python. 
 Doing it in Javascript was a matter of learning the javascript Syntax and apply the same logic has Python. 