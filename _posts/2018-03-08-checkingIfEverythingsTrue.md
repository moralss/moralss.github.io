---
Post:   
Title:  "checking if Everything True"
Date:   2018-03-08
Categories: ""

---
# checking if Everything True

## Introduction 
The reason why im writing this blog post is because of the challenge i faced will
 completed this task working with objects access specific elements inside a object.
## instructions 

The task was to check if every Object in a List had a Key  called Sex which and actual Values like for example male or female , and that i did not have
a value that was falsy.

## Solution 
### code
`

function truthCheck(collection, pre) {

  var counter = 0;
  for (var i in collection) {
    
    if (collection[i].hasOwnProperty(pre) && Boolean(collection[i][pre])) {
      counter++;
    }
  }
  
  return counter == collection.length;
}
console.log(truthCheck([{"user": "Tinky-Winky", "sex": "male"},
 {"user": "Dipsy", "sex": "male"}, {"user": "Laa-Laa", "sex": "female"},
  {"user": "Po", "sex": "female"}], "sex"));

`
 My Function toke in  two parameters  one for the Object and the other for the key . I looped through the object
  parameter and determined if each Object had a property Pre 
 if so it had to a value and it should be a falsy value , if it was true i return true or else i return false.

## conclusion 
Had so much fun doing this task , doing this task taught me how to loop though and object and access  property's .