---
Post:   
Title:  "variable Declaration"
Date:   2018-03-09 14:03:04 -0600
Categories: ""

---
#Variable Declaration

## Introduction 

Writing good quality code in Javascript has been a challenge for me. Specially when it comes to declaring variable names when to use const , var and let.
Looking at my previous code that i wrote in javascript i was using var whenever i was declaring a variable. Making me vulnerably to reassign variables by
mistake. So i think i final understand when to use var , const or let and decided to write a blog post about my understanding. 

## Explanation 

### Var 
lets take a look at the code below 
`
var alertMessage = "hey";
function greetingUser() {
  alertMessage = "hi";
  console.log(alertMessage);
}
greetingUser(); // hi
console.log(alertMessage); // hi

`
alertMessage is a variable i created outside the function storing a string called hey
and i defined the variable as a var, that gives the variable a global scoping (accessible)
so inside my function i had the same alertMessage but i stored a different string value called hi
and so when i console.log alertMessage and console.log the function greetingUser i get the same results hi instead of hey and hi, this is an indication of 
var it beginning accessible globally in your code, allowing you to reassign and remove the previously stored value making var a non-block scoping.      


### Let

The let statement declares a block scope local variable, optionally initializing it to a value.
Variables declared by let have their scope in the block for which they are defined, as well as in any contained sub-blocks.
In this way, let works very much like var.The main difference is that the scope of a var variable is the entire enclosing function. So if you 
dont want your variable to be global you can use let which will provide you with block scoping. 

### Const 

Const is another way of declaring a variable , it can be meaning used for assigning values that don't change after time like for example when i was creating
my tac tic toe game i used const to declare my winning Combinations array. 


## Conclusion 
if you want to know when to use var , let or const then there is a style guide called bnb Style guide .It shows you when its appropriate to use let , const and 
var .





