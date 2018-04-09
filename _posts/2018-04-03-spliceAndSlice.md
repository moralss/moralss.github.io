---
Post:   
Title:  "splice vs Slice"
Date:   2018-03-16
Categories: ""

---
# Splice vs Slice


## Introduction 

The reason why i decided to write a blog post about splice vs Slice , was because of the difficultly i faced when i was busy with a project . The project had to do with creating a
calculator and so i wanted to remove the last element in an array if it ended with operator e.g * -, ? , / , + .  

## Explanation

### Splice 

The splice method changes the contents of an array by removing existing elements and/or adding new elements.
For example if you want to add a element into an array using splice , 
you would use the splice method and pass in three arguments first one representing the index of which you want to insert a new element , second one would be how many elements 
should it remove after the first argument (index) before inserting a new element. 
and your third argument would be the element you want to insert. 
and without the third argument the splice function will only give you the ability to remove elements 



### Slice 

The slice() method returns a shallow copy of a portion of an array into a new array 
object selected from begin to end (end not included). The original array will not be modified.
The slice function takes in two arguments first argument. Is the index of which you want to start slicing , 
and the second argument is until which position index you want to stop 
and it does not include the last index , it does not modify your array so if you want to view the results you are going to have to set the array.slice method in a new variable. 


## Conclusion 

if you want to read more about this topic then heres a link https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/slice






