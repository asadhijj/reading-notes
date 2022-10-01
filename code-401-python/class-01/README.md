# An Introduction To Python 

## Big O 

Big O is a method that is used to evaluate a performence of an algorithim which way to expresses the amount of time that a function, action, or algorithm takes to run based on how many elements we pass to that function. 
so basically we need to look at 2 things when evaluating an algorithim, these 2 things are : 
1.  how much time it requires at runtime
2. how much time and memory it needs.

![Big o](/assets/big%20o.jpeg)

* An O(1) function takes constant time.
* An O(n) function is linear.
* O(n²) function, takes exponentially more time and memory the more elements that you have.

***

## Names & Values in Python 

**Names and values** 
 Names refer to values, a Python assignment statement associates a symbolic name on the left-hand side with a value on the right-hand side, for example : 
```javascript 
x = 20; 
```
but also multiple names can have the same vlaue 
```javascript 
x = 20;
y=x; 
```
in this case y and x have the value of 20
one more important point is that Names are reassigned independently of other names, which means that we can give x a new value but y will still have the old one 

**Assignment** 
 Assignment never copies data, which means that when you assign 2 names with the same value you will have 2 names and 1 value not 2 values !! 
Changes in a value are visible through all of its names, which means that alues fall into two categories based on their type: mutable or immutable. Immutable values include numbers, strings, and tuples. Almost everything else is mutable, including lists, dicts, and user-defined objects. Mutable means that the value has methods that can change the value in-place. Immutable means that the value can never change, instead when you think you are changing the value, you are really making new values from old ones.

Since numbers are immutable, you can't change one in-place, you can only make a new value and assign it to the same name

**Python's Diversity** 
References can be more than just names.it can be Object attributes, list elements and dictionary keys and values, anything on the left side of an operation is considered an assignment.

**Dynamic Typing** 

Names has no type but a scope, you can assign x to an int, then to a float and after that to a string. However, they do have a scope, they come and go with a function for example.

Values have no scope but a type, unlike Names, values to have a type, it could be an int, float or a string, but no scope.

Python is neither "Call By value" nor "Call By Reference", it's "Call by Assignment"!

***
## Awesome Python Environment

Coding in Python is awesome, mainly due to the massive amount of freely available libraries, its readability, and the recently introduced type annotations. 

**The Interpreter**
there are many versions of python that you can install and usee according to your needs.

**Dependency Management**
Managing project dependencies in python can become messy or manual. There exists a bunch of tools to help you with that.

An example of a management tool is poetry.

poetry helps you to easily

    * manage your projects’ dependencies,
    * separate your projects through virtual environments,
    * build both applications as well as libraries without headaches.

**Consistent Formatting and Readability**
Black is a tool for python that allows you to focus on what is necessary, the content. It does that by freeing you from manual code formatting through automation. As it is so nice, let’s add it to our dsexample project and let’s format all files.

**Type-Correctness**
ype annotations are part of the standard library. Through type annotations, your code becomes better to understand, maintain, and less prone to errors
Mypy is a static type checker for python code, that finds errors before they appear. Adding mypy and type-checking to your project using poetry is as easy as adding black.

**Automate the Automation**
Pre-commit is a tool that executes checks before you commit code to your repository (I took for granted that your code is under git version control). When those checks fail, your commit will be rejected. With that, your repository will never see mall formatted code, or none type-checked one, or anything else depending on the checks you are going to include

***

## Things i want to learn mor about 

1. what are we really going to use python for 
2. how are we gonna apply the math and science using python

***
## Sources 

[Big O Notation](https://medium.com/basecs/whats-a-linked-list-anyway-part-2-131d96f71996)

[Names and values in python](https://www.youtube.com/watch?v=_AEJHKGk9ns)

[Python is Awesome](https://towardsdatascience.com/how-to-setup-an-awesome-python-environment-for-data-science-or-anything-else-35d358cc95d5)








