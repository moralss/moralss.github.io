---
Post:
Title:  "setInterval vs Timeout"
Date:   2018-04-09
Categories:

# The difference between setInterval vs setTimeout.


## Introduction 
When i was doing the Pomodoro Clock Challenge i had to decide between the two which one i was going to use , with some research and Theo's Explanation i used the setInterval 
to solve the challenge. 
    
## Explanation 

I figured out the difference between the two, The setTimeout and setInterval are functions that usually take in two arguments one being the mill-seconds the other being a function

that is called , They are considered as 2 timer functions in JavaScript. If you want a function to execute 1 time then you can use a setTimeout(),
 
if you want to execute a function unlimited times then use setInterval() ,the function will execute for every mill-second that's passed in , and you can stop the execution be saying clearInterval.  

 
## solution 
This is how i used the setTimeout() in my code to solve this challenge.

`
var SessionInterval = setInterval(SessionDecreaseTimer, 1000);

function SessionDecreaseTimer() {
    breakTime--;
    if (breakTime <= 0) {
        clearInterval(SessionInterval);
    };

    updateClockDisplay("breakOutput", breakTime);
}


`


## Conclusion 
I couldn't use the setTimeout() function because my Pomodoro clock needed to count down , by doing so i needed a function that could execute unlimited times for every second 
until i tell it to stop. So that's why i went with the setInterval it worked perfectly for the Pomodoro Clock. 