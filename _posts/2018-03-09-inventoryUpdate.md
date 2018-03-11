---
Post:   
Title:  "Updating inventory"
Date:   2018-03-09
Categories: ""

---
# Update inventory

## Introduction 
The reason why i choice to wrote a blog post about this challenge , a challenge i got from FreeCodeCamp .Was because of the difficulties i faced when completing this challenge , 
it was my first time using 2 dimensional arrays , it was one of the reasons why i battled because i was not familiar with Javascript 2 dimensional arrays   

## Instructions 

Compare and update the inventory stored in a 2D array against a second 2D array of a fresh delivery. Update the current existing inventory item quantities (in arr1). 
If an item cannot be found, add the new item and quantity into the inventory array. The returned inventory array should be in alphabetical order by item.


## Solution 
### Code
`

function updateInventory(arr1, arr2) {
    for (var i in arr2) {
        var existing = arr1.every(function (element) {
            return arr2[i][1] !== element[1]
        });
        if (existing) {
            arr1.push(arr2[i]);
        }
            arr1.forEach(function (element) {
                if (element.indexOf(arr2[i][1]) !== -1) {
                    element[0] = element[0] + arr2[i][0]
                }
            });
    }
    return arr1.sort((a , b ) => (a[1] < b[1]) ? -1 : 1);
}

// Example inventory lists
var curInv = [
    [21, "Bowling Ball"],
    [2, "Dirty Sock"],
    [1, "Hair Pin"],
    [5, "Microphone"]
];

var newInv = [
    [2, "Hair Pin"],
    [3, "Half-Eaten Apple"],
    [67, "Bowling Ball"],
    [7, "Toothpaste"]
];


`
I created a function UpdateInvetory that toke in two arrays each was a 2 dimensional array storing the points and name. I then compared the first array with the seconded array to try and see if their is a match if not i updated the 
inventory with the element that had no match . If there was a match and then accessed the first index and added the two scores together.  
## Conclusion 

First true challenge i had with two dimensional array. learnt alot for this challenge and going to continue learning more ! 











