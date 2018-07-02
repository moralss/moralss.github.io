
---
Post:   
Title:  "working with local storage"
Date:   2018-06-28
Categories: ""

---

## Introduction 
When I was busy building a recipe box, I had to use local storage to save
my recipes. In this blog post, I am going to show you how to use local storage and what local storage really is.  


## 4 what is a browser local storage

local storage is a component of the Web storage application programming interface. It is a method by which Web pages locally store named key/value pairs inside a client's Web browser. ... Local storage is mainly used to store and retrieve data in HTML pages from the same domain.

## how to incorporate local storage in your application
they are certain key factors for incorporating local storage to your website,
first, you have to understand the code that you need to store data to local storage and the other one is how to read data from local storage. Let me elaborate using 
an example I had when creating the recipe box my recipes and ingredients were 
in key-value pairs and so what I did in my code was I stored my object  as 
follows : 
`

localStorage.setItem('recipes', JSON.stringify(customerRecipes));

`
by saying localStorage.setItem you're specifying that you want to store a data,
the first argument you are naming your local store, the second argument you are passing in what you want to store but you have to specify the datatype to be stored a  string.

if you want to get data the code needed is as follows :

localStorage.getItem('newRecipe');

instead of using the method setItem you use a different method called getItem 
which retrieves data from local storage.

## Conclusion 

It's not  hard to store data in local storage, you just need to understand 
setItem and getItem methods. when setting and getting data from local storage
