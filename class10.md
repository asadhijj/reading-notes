## In memory storage 

An in-memory database (IMDB) stores computer data in a computer's main memory instead of a disk drive to produce quicker response times. Accessing data stored in memory eliminates the time needed to query data from a disk.

*** 
## JS call stack

1. **What is a 'call'?**
 is a data structure that uses the Last In, First Out (LIFO) principle to temporarily store and manage function invocation (call).

 2. **How many 'calls' can happen at once?**
 one at a time.

 3. **What does LIFO mean?**
  When we say that the call stack, operates by the data structure principle of Last In, First Out, it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.

  4. **Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.**

  ![Invoked](./assets/stack.png)

  5. **What causes a Stack Overflow?**
  A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error.

  ***

  ## JS Error Message 

  1. **What is a 'reference error'?**
  This is as simple as when you try to use a variable that is not yet declared you get this type os errors.

  2. **What is a 'syntax error'?**
   this occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.

   3. **What is a 'range error'?**
   occurs when giving an object or an array an invalid lenght 

   4. **What is a 'type error'?**
   this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.

   5. **What is a breakpoint?**
   A breakpoint is a point in the program where the code will stop executing.

   6. **What does the word 'debugger' do in your code?**
   identifying coding errors at various stages of the operating system or application development. 


   ***

    ## Things I want to know more about
    nothing for this class.

    *** 
    ## External Sources 

    [call stack](https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4)

    [Errors](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)

