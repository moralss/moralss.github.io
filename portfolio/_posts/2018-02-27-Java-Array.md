
---
Post:   
Title:  "Java Array"
Date:   2019-02-27
Categories: ""

---

## Introduction 

Today I'm going to share with you the two ways you can create an array in Java and the benefits of using ArrayList then just using a normal array. 

## body

There are two ways of declaring arrays In Java. The example below shows this two ways. 

### example 1.
String[] cars.

### example 2.
ArrayList<String> cars = new ArrayList<String>();


Example1 declares an array by specifying the data type String with square brackets followed by the name of the list.
Example2 uses an ArrayList which can be found in the java. util package.  

## Advantages
the Advantages of using ArrayList.

You can define ArrayList as a re-sizable array. Size of the ArrayList is not fixed. ArrayList can grow and shrink dynamically.
if generics are not used, ArrayList can hold any type of objects.
ArrayList is also proven to be faster than arrays.
ArrayList class has many methods to manipulate the stored objects.
An example can be the set method which updates the store. by passing in two parameters the index of the value you want to replace and the value you want to replace it with. The add method which adds to the array. and many more different method.  

## Conclusion 
 
I prefer using ArrayList instead of a normal array list when working with arrays.