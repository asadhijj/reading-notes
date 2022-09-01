# Functional Programming 

Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data.

***

## Functional Programming Concepts 

1. **What is functional programming?** 
Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data.

2. **What is a pure function and how do we know if something is a pure function?**
    -It returns the same result if given the same arguments (it is also referred as deterministic)
    -It does not cause any observable side effects
we can distinguish a pure function by looking at these attributes :
    *It returns the same result if given the same arguments
    * Reading Files (If function reads external files, it’s not a pure function)
    *Random number generation (Any function that relies on a random number generator cannot be pure.)
    * It does not cause any observable side effects
    

3. **What are the benefits of a pure function?**
    -Given a parameter A → expect the function to return value B
    -Given a parameter C → expect the function to return value D

4. **What is immutability?**
When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.

5. **What is Referential transparency?**
if a function consistently yields the same result for the same input, it is referentially transparent.


***

## Module and Require 

1. **What is a module**
it is a javascript file that is used to make the code cleaner by putting the function of task in that module seperating it from its rendering.

2. **What does the word 'require' do ?**
allows us to use a function elsewhere in the application.

3. **How do we bring another module into the file the we are working in?**
by typing 
```javascript 
require ('./fileName') // passing the path of the module within the string inside require.
```
4. **What do we have to do to make a module available?**
 ```javascript 
 module.exports = Whatever we want available outside the modul; 
```

***
 ## Things I want to know more about
 i want to get a better idea about servers and how they specifically do all the job (requests and responds)

 *** 
 ## External Sources 
 [Functional Programming](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)

 [Moduels and require](https://www.youtube.com/watch?v=9UaZtgB5tQI)