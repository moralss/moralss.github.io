---
Post:   
Title:  "Switch Statement"
Date:   2018-03-16
Categories: ""

---
# Converting Html


## Introduction 

Used a Switch Statement in an efficient way. 

## Instructions 
Convert the characters &, <, >, " (double quote), and ' (apostrophe), in a string to their corresponding HTML entities.



## Solution 
### Code

`

function convertHTML(str) {
  
  var temp = str.split('');


  for (var i = 0; i < temp.length; i++) {
    switch (temp[i]) {
      case '<':
        temp[i] = '&lt;';
        break;
      case '&':
        temp[i] = '&amp;';
        break;
      case '>':
        temp[i] = '&gt;';
        break;
      case '"':
        temp[i] = '&quot;';
        break;
      case "'":
        temp[i] = "&apos;";
        break;
    }
  }

  temp = temp.join('');
  return temp;
}


`


Switch statement passes in a value followed by curly braces instead the curly braces you get the word Case followed by a element representing what you pass in as a value ,
underneath it you basically tell it that if the element
is passed in with a specific name then do the process that follows ? 


## Conclusion 

i never really fully understood switch statements in Javascript until i decided to write it down and explained it to myself , and by also looking at the memo for this exercise on forum . no i think i fully do 

and the power of using it.   








