---
Post:   
Title:  "regularExpressions"
Date:   2018-05-08
Categories: ""

---
# regular Expressions

## Introduction 
Using regular expressions makes getting , filtering information in a string much easier.I decided to write a blog post and share 
some of the regex Expressions you can use to filter information.



## Definition
 a sequence of symbols and characters expressing a string or pattern to be searched for within a longer piece of text. 


## Explains 

If you have a string that consists of numbers , letters and digits , and you wanted to get all the digits in that particular string.You can
use a regex expressions,but first you need to define the string variable name and store same text , or hard code the string  followed by the .match function and in brackets type in your regex expression for filtering digits and thats a  /\d/g , which is basically two forward slashes followed by a g which stands 
for global go through every character in the string , and in between the forward slashes its a back slash followed by a d representing digits. If you 
wanted all the small letters you could have replaced the \d with a [a-z]. And for all the capital letters and small letters you could have used [a-zA-z]
in the  place of [a-z] , or you could have just changed the g with an i which means  ignore case sensitive.     


## Code Explains 
basic regex Expressions for filtering myString.match(/\d/g);

let regexSmallLetters = /[a-z]/g;
let regexNumbers = /\d/g;
let regexAllLetters = /[a-zA-Z]/g;
let regexWhiteSpacing = /\ /g;

## Conclusion 

Regex makes it easier to filter characters in a string. The filtered results get thrown back as an array.  
