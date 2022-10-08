# FileIO & Exceptions

## Files 

a file is a contiguous set of bytes used to store data. This data is organized in a specific format and can be anything as simple as a text file or as complicated as a program executable. In the end, these byte files are then translated into binary 1 and 0 for easier processing by the computer.

Files on most modern file systems are composed of three main parts:

    * Header: metadata about the contents of the file (file name, size, type, and so on)
    * Data: contents of the file as written by the creator or editor
    * End of file (EOF): special character that indicates the end of the file

**File paths**
The file path is a string that represents the location of a file. It’s broken up into three major parts:

    1. Folder Path: the file folder location on the file system where subsequent folders are separated by a forward slash / (Unix) or backslash \ (Windows)
    2. File Name: the actual name of the file
    3. Extension: the end of the file path pre-pended with a period (.) used to indicate the file type

**Opening and Closing a File in Python**

you can open a file using the command : 
```python 
file = open('dog_breeds.txt')
```

to read and close the file : 

```python 
reader = open('dog_breeds.txt')
try:
    # Further file processing goes here
finally:
    reader.close()
```


or : 

```python 
with open('dog_breeds.txt') as reader:
    # Further file processing goes here
```

you can choose the mode of which the file you want to be opened with by using the following : 



|Character   |Meaning                                                  |
|------------|---------------------------------------------------------|
|'r'         |Open for reading (default)                               |
|'w' 	       |Open for writing, truncating (overwriting) the file first|
|'rb' or 'wb'|Open in binary mode (read/write using byte data)         |




**Types Of Files** 
There are three different categories of file objects:

    * Text files -> open('abc.txt')
    * Buffered binary files -> open('abc.txt', 'rb')
    * Raw binary files -> open('abc.txt', 'rb', buffering=0)


***

## Exception in Python 

Syntax errors occur when the parser detects an incorrect statement, but exception error occurs whenever syntactically correct Python code results in an error.

We can use raise to throw an exception if a condition occurs. The statement can be complemented with a custom exception.

example : 
```python 
x = 10
if x > 5:
    raise Exception('x should not exceed 5. The value of x was: {}'.format(x))

```

**The AssertionError Exception**

We assert that a certain condition is met. If this condition turns out to be True, then that is excellent! The program can continue. If the condition turns out to be False, you can have the program throw an AssertionError exception.


**The try and except Block: Handling Exceptions**

The try and except block in Python is used to catch and handle exceptions. Python executes code following the try statement as a “normal” part of the program. The code that follows the except statement is the program’s response to any exceptions in the preceding try clause.



**The else Clause**

In Python, using the else statement, you can instruct a program to execute a certain block of code only in the absence of exceptions.


**Cleaning Up After Using finally**

Imagine that you always had to implement some sort of action to clean up after executing your code. Python enables you to do so using the finally clause.

![Diagram summing up the process](https://files.realpython.com/media/try_except_else_finally.a7fac6c36c55.png)


***

## Sources 

[Files](https://realpython.com/read-write-files-python/)

[Exception](https://realpython.com/python-exceptions/)
[Video](https://realpython.com/courses/reading-and-writing-files-python/)

*** 
## Things i want to learn more about 

1. why do we need to open, read files in python 
2. how to use the exception process in a real code

