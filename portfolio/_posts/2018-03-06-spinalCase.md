---
Post:   
Title:  "regex"
Date:   2018-02-09
Categories: ""

---
# Spinal Case  

## Introduction 
The reason why i'm writing this blog post is to share what i have learned form this challenge i got 
from FreeCodeCamp. 
## instructions 

the challenge instructed me to Convert a string to spinal case. Spinal case is all-lowercase-words-joined-by-dashes.


## Solution 
### code
`

function spinalCase(str) {
//   var whiteSpacing = str.match(/\s/g);

  var res = str.replace(/([a-z])([A-Z])/g,'$1-$2' );

  return res.toLowerCase().replace(/\W|_/g,'-');

}

console.log(spinalCase('This Is Spinal Tap'));


`
 
I learnt about regex and the meaning of regex. The definition of regex is a , regular expression (sometimes abbreviated to "regex") is a way for a computer user or programmer to express how a computer program should look for a specified pattern in text and then what the program is to do when each pattern match is found. For example, a regular expression could tell a program to search for all text lines that contain the word "Windows 95" and then to print out each line in which a match is found or substitute another text sequence (for example, just "Windows") where any match occurs.

So this method allowed me to get white spacing and allowed me to separate words that where combined . 
## conclusion 

I feel like this concept of using regex is a very important concept that can even help you check for password validation. it was fun learning this concept and i hope i make it stuck. 