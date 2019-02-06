---
Post:   
Title:  "simonGame"
Date:   2018-05-15
Categories: ""

---
# simonGame


## Introduction 
In this blog post, I'm going to share with the methods and logic I took in solving the Simon Game.

 ##Instructions  

The device has four coloured buttons, each producing a particular tone when it is pressed or activated by the device. Around in the game consists of the device lighting up one or more buttons in a random order, after which the player must reproduce that order by pressing the buttons. As the game progresses, the number of buttons to be pressed increases.
ref = https://en.wikipedia.org/wiki/Simon_(game)

## Solution 

I started off by finding a way in which my buttons would flick on and off, I did that by using a setInterval function and 
a setTimeout Function, to handle the flicking put. Also found a way to generate a random number from 0 to 3 in which each number will be linking to the colours red, blue, green and yellow. Basically for each stage completed I generate a new random number
and add it to the computerColorMoves array. I checked if the computer's moves was the same as the players moves , I managed to 
figure that out by looping through the users move and comparing each value with the value of the computer moves and if it is the same 
and the lengths are also the same then the user has completed the sequence and a new random number is generate and pushed into the computerColorMoves array. When the user has reached his twentieth move than an alert will display showing him that he has won the game.


## Conclusion 

it took me time to figure out the logic, but I managed to come up with a solution and solved the Simon Game. I had fun working on this 
project.
