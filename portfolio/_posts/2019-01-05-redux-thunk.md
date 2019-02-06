
---
Post:   
Title:  "Redux Thunk"
Date:   2019-01-05
Categories: ""

---

## Introduction 

Whats Redux Thunk? so before you can understand redux thunk you first need to know what Redux is and what problem does redux thunk solve. 

## body

So Whats Redux? While Redux is a predictable state container for JavaScript apps.
but Redux alone without any Redux middleware is not good enough when your Frontend App is making calls to a server somewhere, you are going to need to create asynchronous action creators.
 because Redux alone can only do that much example when creating an action creator it as to be a function that returns a javascript object, that's why we use Redux Thunk. Redux Thunk is a Redux middleware that allows us to create action
creators that return a function instead of an action object.
Therefore you can create a thunk that returns a function for a successful request by returning an object with the data from the server. If retrieving the data was an unsuccessful request then you can return a function which cantains an object with the errors received from the server.

## Conclusion 

That's not the only way to deal with asynchronous action creators. There is also Redux Saga which uses generator functions. 