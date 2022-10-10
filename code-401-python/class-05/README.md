# Intro to OOP

Object-oriented programming (OOP) is a method of structuring a program by bundling related properties and behaviors into individual objects. In this tutorial, you’ll learn the basics of object-oriented programming in Python.

Conceptually, objects are like the components of a system. Think of a program as a factory assembly line of sorts. At each step of the assembly line a system component processes some material, ultimately transforming raw material into a finished product.

An object contains data, like the raw or preprocessed materials at each step on an assembly line, and behavior, like the action each assembly line component performs.

## Classes and Objects 

Objects are an encapsulation of variables and functions into a single entity. Objects get their variables and functions from classes. Classes are essentially a template to create your objects.

you can make your object using "myobjectx = Class()" and you acn access the variables inside of the class by using "myobjectx.variable" and to access functions "myobjectx.function"

Also, You can create multiple different objects that are of the same class(have the same variables and functions defined). However, each object contains independent copies of the variables defined in the class

The __init__() function, is a special function that is called when the class is being initiated. It's used for assigning values in a class.


*** 

## Thinkin Recursively 

A recursive function is a function defined in terms of itself via self-referential expressions.

 the function will continue to call itself and repeat its behavior until some condition is met to return a result. All recursive functions share a common structure made up of two parts: base case and recursive case. 

to maintain state during recursion you have to either:

    * Thread the state through each recursive call so that the current state is part of the current call’s execution context
    * Keep the state in global scope

A data structure is recursive if it can be deﬁned in terms of a smaller version of itself. A list is an example of a recursive data structure


we use the lru_cache which is a decorator that help to avoid recomputation by explicitly checking for the value before trying to compute it.


## Pytest Fixtures and Coverage 

**Fixtures**

Fixtures are objects that can be available to all your tests and these objects might contain data or they might involve the network or filesystem and they come in variety in forms.

Fixtures define the steps and data that constitute the arrange phase of a test . In pytest, they are functions you define that serve this purpose. They can also be used to define a test’s act phase; this is a powerful technique for designing more complex tests.

The services, state, or other operating environments set up by fixtures are accessed by test functions through arguments. For each fixture used by a test function there is typically a parameter (named after the fixture) in the test function’s definition.

We can tell pytest that a particular function is a fixture by decorating it with @pytest.fixture. 

pytest does its best to put all the fixtures for a given test in a linear order so that it can see which fixture happens first, second, third, and so on. If an earlier fixture has a problem, though, and raises an exception, pytest will stop executing fixtures for that test and mark the test as having an error.

When a test is marked as having an error, it doesn’t mean the test failed, though. It just means the test couldn’t even be attempted because one of the things it depends on had a problem.

This is one reason why it’s a good idea to cut out as many unnecessary dependencies as possible for a given test. That way a problem in something unrelated isn’t causing us to have an incomplete picture of what may or may not have issues.


**Coverage**

code coverage helps you notice missing things in your code when the code is large and complex which gives a better confidence in your code that it has run at least once 

here's a package called pytest-cov on PyPI

you can invoke pytest with the --cov option. but this option will give coverage for every part of the python library your code used, so it is suggested to provide 
an argument to --cov, specifying which program(s) you want to test. And, you should indicate the directory into which the report should be written

for example : 

```python 
pytest --cov=mymul .
```

you'll need to turn the coverage report into something human-readable, so use : 
 
```python 
coverage html
```


***

## Sources 

1. [Classes and objects](https://www.learnpython.org/en/Classes_and_Objects)

2. [Thinking Recursively](https://realpython.com/python-thinking-recursively/)

3. [Fixtures and Coverage](https://www.linuxjournal.com/content/python-testing-pytest-fixtures-and-coverage)


***

## Things i want to learn more about 

1. How to use Fixtures and Coverage in a real complex test 

2. how to recursive functions can be used in a process to make a program 

