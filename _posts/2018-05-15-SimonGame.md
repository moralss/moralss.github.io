---
Post:   
Title:  "simonGame"
Date:   2018-05-15
Categories: ""

---
# simonGame

## Introduction 
In this blog post im going to share with the methods and logic i took in solving the Simon Game.

 ##Instructions  

The device has four colored buttons, each producing a particular tone when it is pressed or activated by the device. A round in the game consists of the device lighting up one or more buttons in a random order, after which the player must reproduce that order by pressing the buttons. As the game progresses, the number of buttons to be pressed increases.
ref = https://en.wikipedia.org/wiki/Simon_(game)

## Solution 

So i started off by finding a way in which my buttons would flick on and off ,i did that by using a setInterval function and 
a setTimeout Function , to handle the flicking put. Also found a way to generate a random number from 0 to 3 in which each number 
will be linking to the colors red ,  blue , green and yellow. Basically for each stage completed i generate a new random number
and add it to the computerColorMoves array. I checked if the computers moves was the same as the players moves , i managed to 
figure that out by looping through the users move and comparing each value with the value of the computer moves and if it is the same 
and the lengths are also the same then the user has completed the sequence and a new random number is generate and pushed into the computerColorMoves array.When the user as reached his twentieth move than an alert will display showing him that he as won the game.


## Conclusion 

it took me time to figure out the logic ,but i managed to came up use a solution and solved the Simon Game. I had fun working on this 
project.




