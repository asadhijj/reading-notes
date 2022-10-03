# Testing And Modules 

## Testing 
 
 first of all we use testing to try our input and output and the how the code actually runs 

this is done by writing a piece of code to check if we get the expected output depending on the input but first of all we need to identify what we actually need the output to be and what should the input be.
there are some steps that must be followed, which they are : 
 1. the test file should be given the same name as the module file 
 2. the structure used for the process (AAA) should be as the following : 
 - Arrange : you need to organize the data needed to execute that piece of code (input)
 - Act : here you will execute the code being tested (exercise the behaviour)
 - Assert : after executing the code, you will check if the result (output) is the same as you were expecting.

 **The Cycle of testing**
 first of all you should write a code to fail the test so you know the testing method is working, then try to give an input that should pass and if it passes this means that the test is working, lastly you have to refactor the code to make it look more readable and neater. 


 **TDD** 
 Test Design Driven just means that when we make a testing method the method should be working with the whole software design and not just a single unit of input. 


 ***

 ## If Name Equals Main 

 If the python interpreter is running that module (the source file) as the main program, it sets the special __name__ variable to have a value “__main__”. If this file is being imported from another module, __name__ will be set to the module’s name. Module’s name is available as value to __name__ global variable. 

 so if we use the __name__ == __main__ on a specific block on a module when the code is run that module should be the entry point otherwise the specific block of the code will not run. 

 **Advantages :**

    1.Every Python module has it’s __name__ defined and if this is ‘__main__’, it implies that the module is being run standalone by   the user and we can do corresponding appropriate actions.
    2. If you import this script as a module in another script, the __name__ is set to the name of the script/module.
    3. Python files can act as either reusable modules, or as standalone programs.
    4. if __name__ == “main”: is used to execute some code only if the file was run directly, and not imported. 


***

## Recursion 

Recursion is The process in which a function calls itself directly or indirectly is called recursion and the corresponding function is called a recursive function.
 we need recursion because it can reduce the length of our code and make it easier to read and write

**Properties of Recursion:**

    - Performing the same operations multiple times with different inputs.
    - In every step, we try smaller inputs to make the problem smaller.
    - Base condition is needed to stop the recursion otherwise infinite loop will occur.

Recursion can be used to solve a particular problem by represnting the problem in one or more smaller problems and giving a base solution to get out of the recursive state.

**Memory Allocation to Multiple Function Calls** 
When any function is called from main(), the memory is allocated to it on the stack. A recursive function calls itself, the memory for a called function is allocated on top of memory allocated to the calling function and a different copy of local variables is created for each function call. When the base case is reached, the function returns its value to the function by whom it is called and memory is de-allocated and the process continues.

***

## Python Lists 

List are written within square brackets [ ]. Lists work similarly to strings -- use the len() function and square brackets [ ] to access data, with the first element at index 0.

so for example if we have a list called "colors" and then assigned it to another variable called "x" that doesnt mean we have a copy of the list, it means that both of these (colors and x) point to the same list.

we can also append 2 lists together by using the "+" sign => [1,2] + [3,4] = [1,2,3,4]

**FOR and IN**
for var in list -- is an easy way to look at each element in a list (or other collection)

we can use value in collection -- tests if the value is in the collection, returning True/False.


**Range**
The range(n) function yields the numbers 0, 1, ... n-1, and range(a, b) returns a, a+1, ... b-1 -- up to but not including the last number.

**While Loop**
Python also has the standard while-loop, and the *break* and *continue* statements work as in C++ and Java, altering the course of the innermost loop. The above for/in loops solves the common case of iterating over every element in a list, but the while loop gives you total control over the index numbers.


**List Methods**
* list.append(elem) -- adds a single element to the end of the list. Common error: does not return the new list, just modifies the original.
* list.insert(index, elem) -- inserts the element at the given index, shifting elements to the right.
* list.extend(list2) adds the elements in list2 to the end of the list. Using + or += on a list is similar to using extend().
* list.index(elem) -- searches for the given element from the start of the list and returns its index. Throws a ValueError if the element does not appear (use "in" to check without a ValueError).
* list.remove(elem) -- searches for the first instance of the given element and removes it (throws ValueError if not present)
* list.sort() -- sorts the list in place (does not return it). (The sorted() function shown later is preferred.)
* list.reverse() -- reverses the list in place (does not return it)
* list.pop(index) -- removes and returns the element at the given index. Returns the rightmost element if index is omitted (roughly the opposite of append())

we can also use list slices just like strings to change sub-parts of the list.

***

## Python Strings 

Python has a built-in string class named "str" with many handy features (there is an older module named "string" which you should not use).
Python strings are "immutable" which means they cannot be changed after they are created (Java strings also use this immutable style)
Characters in a string can be accessed using the standard [ ] syntax.

**String Methods**


    * s.lower(), s.upper() -- returns the lowercase or uppercase version of the string
    * s.strip() -- returns a string with whitespace removed from the start and end
    * s.isalpha()/s.isdigit()/s.isspace()... -- tests if all the string chars are in the various character classes
    * s.startswith('other'), s.endswith('other') -- tests if the string starts or ends with the given other string
    * s.find('other') -- searches for the given other string (not a regular expression) within s, and returns the first index where it begins or -1 if not found
    * s.replace('old', 'new') -- returns a string where all occurrences of 'old' have been replaced by 'new'
    * s.split('delim') -- returns a list of substrings separated by the given delimiter. The delimiter is not a regular expression, it's just text. 'aaa,bbb,ccc'.split(',') -> ['aaa', 'bbb', 'ccc']. As a convenient special case s.split() (with no arguments) splits on all whitespace chars.
    * s.join(list) -- opposite of split(), joins the elements in the given list together using the string as the delimiter. e.g. '---'.join(['aaa', 'bbb', 'ccc']) -> aaa---bbb---ccc

**String Slices**

The "slice" syntax is a handy way to refer to sub-parts of sequences -- typically strings and lists. The slice s[start:end] is the elements beginning at start and extending up to but not including end

**String Formatting**

One neat thing python can do is automatically convert objects into a string suitable for printing. Two built-in ways to do this are formatted string literals, also called "f-strings", and invoking str.format().

Python also has an older printf()-like facility to put together a string. The % operator takes a printf-type format string on the left (%d int, %s string, %f/%g floating point), and the matching values in a tuple on the right (a tuple is made of values separated by commas, typically grouped inside parentheses):
  # % operator
  ```python
  text = "%d little pigs come out, or I'll %s, and I'll %s, and I'll blow your %s down." % (3, 'huff', 'puff', 'house')
  ```


## python Modules And Packages 

Modular programming refers to the process of breaking a large, unwieldy programming task into separate, smaller, more manageable subtasks or modules. Individual modules can then be cobbled together like building blocks to create a larger application.

**Advantages of Modularization**

* Simplicity
* Maintability
* Reusability
* Scoping

Functions, modules and packages are all constructs in Python that promote code modularization.

**Packages**

Packages allow for a hierarchical structuring of the module namespace using dot notation. In the same way that modules help avoid collisions between global variable names, packages help avoid collisions between module names.


***

## Pytest 

The pytest framework makes it easy to write small, readable tests, and can scale to support complex functional testing for applications and libraries.


**Some of the advantages of pytest are**

   * Very easy to start with because of its simple and easy syntax.
   * Can run tests in parallel.
   * Can run a specific test or a subset of tests
   * Automatically detect tests
   * Skip tests
   * Open source

**Assertion In PyTest**

Pytest assertions are checks that return either True or False status. In Python Pytest, if an assertion fails in a test method, then that method execution is stopped there. The remaining code in that test method is not executed, and Pytest assertions will continue with the next test method.

example => assert 4==4 is a successful assertion



* By default pytest only identifies the file names starting with test_ or ending with _test as the test files, Pytest requires the test method names to start with “test.” All other method names will be ignored even if we explicitly ask to run those methods.

example => 
test_login.py - valid
login_test.py - valid
testlogin.py -invalid
logintest.py -invalid

* if we have a folder with multiple test files we can run all of them by writing the command : 
```py.test``` (which will run only the filenames starting with test_ and the filenames ending with _test in that folder and subfolders under that folder.)

* if we want to run a specific test file in the folder we can write the command : 
```py.test test_sample1.py```

* Sometimes we don’t want to run the entire test suite. Pytest allows us to run specific tests. We can do it in 2 ways

    - Grouping of test names by substring matching
    - Grouping of tests by markers


* Fixtures are used when we want to run some code before every test method. So instead of repeating the same code in every test we define fixtures. Usually, fixtures are used to initialize database connections, pass the base , etc
code line : 
```@pytest.fixture```

* Parameterized Test -> The purpose of parameterizing a test is to run a test against multiple sets of arguments. We can do this by ```@pytest.mark.parametrize```


* There will be some situations where we don’t want to execute a test, or a test case is not relevant for a particular time. In those situations, we have the option to Xfail the test or skip the tests

The xfailed test will be executed, but it will not be counted as part failed or passed tests. There will be no traceback displayed if that test fails. We can xfail tests using

```@pytest.mark.xfail```

Skipping a test means that the test will not be executed. We can skip tests using

```@pytest.mark.skip```


## Things i want to learn more about 

1. what are we really going to use python for 
2. i am curious about the functionality of Pytest in a real code application
3. usage of lists and tuples 

***

## Sources 

[Testing and TDD](https://code.likeagirl.io/in-tests-we-trust-tdd-with-python-af69f47e6932)

[If name equals main](https://www.geeksforgeeks.org/what-does-the-if-__name__-__main__-do/)

[Recursion](https://www.geeksforgeeks.org/introduction-to-recursion-data-structure-and-algorithm-tutorials/)

[Lists](https://developers.google.com/edu/python/lists)

[strings](https://developers.google.com/edu/python/strings)

[Modules and Packages](https://realpython.com/python-modules-packages/)

[Pytest](https://www.guru99.com/pytest-tutorial.html)