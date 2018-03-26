---
Layout:
Title: "caesarsCipher"
Date: 2018-02-08
Categories:

---
# caesarsCipher

## Introduction

i tried completing this exercise with the shortest possible way. Making it easy to explain. 

## Explanation 
`

function rot13(str) {
    var temp = [];
    var myListOfAlphabets = ["A", "B", "C", "D", "E", "F", "G", "H", "I", "J", "K", "L", "M", "N", "O", "P", "Q", "R", "S", "T", "U", "V", "W", "X", "Y", "Z", "A", "B", "C", "D", "E", "F", "G", "H", "I", "J", "K", "L", "M"]
    var splitString = str.split('');

    for (var i = 0; i < splitString.length; i++) {
        if (myListOfAlphabets.indexOf(splitString[i]) === -1) {
            temp.push(splitString[i]);
        }
        else {
            for (var j = 0; j < myListOfAlphabets.length; j++) {
                if (splitString[i] === myListOfAlphabets[j]) {
                    temp.push(myListOfAlphabets[j + 13]);
                }
            }
        }
    }

    return temp.join("");

}

`

i started by creating a function called Rot13 , that takes in a string as an argument called str. Inside the function i created a temp array which i set to 
an empty array , followed by a array i called myListOfAlphabets which stores all the alphabets from A to Z and A to M taking up 39 spots in the array. 
i then created a variable called SplitString which splitted the string argument and converted it into an array of char characters , i looped through the 
splitted string characters and wrote a conditional statement which checked if the char characters in  myListOfAlphabets had a letter equal to the
 splitted string character if not and then pushed it to my empty array i defined as temp. Else i toke the character of the splittedString array that was equal
  to the mylistOfAlphabets array and moved each character of the splittedString array 13 places forward. according to the mylistOfAlphabets array.

## conclusion

i used a for loop , conditional statement , .join() function and the .split() function to solve this challenge.

  

