# Data Structures

A data structure is a specialized format for organizing, processing, retrieving and storing data. There are several basic and advanced types of data structures, all designed to arrange data to suit a specific purpose. Data structures make it easy for users to access and work with the data they need in appropriate ways. Most importantly, data structures frame the organization of information so that machines and humans can better understand it.


**Why are data structures important?**

Typical base data types, such as integers or floating-point values, that are available in most computer programming languages are generally insufficient to capture the logical intent for data processing and use. Yet applications that ingest, manipulate and produce information must understand how data should be organized to simplify processing. Data structures bring together the data elements in a logical way and facilitate the effective use, persistence and sharing of data. They provide a formal model that describes the way the data elements are organized.


## Data Structure Usage and its Types 

In general, data structures are used to implement the physical forms of abstract data types. Data structures are a crucial part of designing efficient software. They also play a critical role in algorithm design and how those algorithms are used within computer programs.


examples of how data structures are used include the following:

   * Storing data. Data structures are used for efficient data persistence, such as specifying the collection of attributes and corresponding structures used to store records in a database management system.

   * Managing resources and services. Core operating system (OS) resources and services are enabled through the use of data structures such as linked lists for memory allocation, file directory management and file structure trees, as well as process scheduling queues.

   * Data exchange. Data structures define the organization of information shared between applications, such as TCP/IP packets.

   * Ordering and sorting. Data structures such as binary search trees -- also known as an ordered or sorted binary tree -- provide efficient methods of sorting objects, such as character strings used as tags. With data structures such as priority queues, programmers can manage items organized according to a specific priority.

   * Indexing. Even more sophisticated data structures such as B-trees are used to index objects, such as those stored in a database.

   * Searching. Indexes created using binary search trees, B-trees or hash tables speed the ability to find a specific sought-after item.

   * Scalability. Big data applications use data structures for allocating and managing data storage across distributed storage locations, ensuring scalability and performance. Certain big data programming environments -- such as Apache Spark -- provide data structures that mirror the underlying structure of database records to simplify querying.


**Characteristics of data structures**

Data structures are often classified by their characteristics. The following three characteristics are examples:

   * Linear or non-linear. This characteristic describes whether the data items are arranged in sequential order, such as with an array, or in an unordered sequence, such as with a graph.

   * Homogeneous or heterogeneous. This characteristic describes whether all data items in a given repository are of the same type. One example is a collection of elements in an array, or of various types, such as an abstract data type defined as a structure in C or a class specification in Java.

   * Static or dynamic. This characteristic describes how the data structures are compiled. Static data structures have fixed sizes, structures and memory locations at compile time. Dynamic data structures have sizes, structures and memory locations that can shrink or expand, depending on the use.


**Data Types**

* Boolean : Logical Values (True or False)

* Integer : range on mathematical integers -- or counting numbers

* Floating-point numbers : formulaic representation of real numbers

* Fixed-Point Number : hold real values but are managed as digits to the left and the right of the decimal point.

* Character : Symbols to define something else

* Pointers : Reference values that point to other values

* String : An array of characters


![The data structure hierarchy shows how data types and data structures are related. ](https://cdn.ttgtmedia.com/rms/onlineimages/whatis-data_structure.png)


**Types of Data Structures**

* Array : stores a collection of items at adjoining memory locations. Items that are the same type are stored together so the position of each element can be calculated or retrieved easily by an index. Arrays can be fixed or flexible in length.

* Stack : stores a collection of items in the linear order that operations are applied. This order could be last in, first out (LIFO) or first in, first out (FIFO).

* Queue :  stores a collection of items like a stack; however, the operation order can only be first in, first out.

* Linked List : stores a collection of items in a linear order. Each element, or node, in a linked list contains a data item, as well as a reference, or link, to the next item in the list.

* Tree : stores a collection of items in an abstract, hierarchical way. Each node is associated with a key value, with parent nodes linked to child nodes -- or subnodes. There is one root node that is the ancestor of all the nodes in the tree.

* Heap : is a tree-based structure in which each parent node's associated key value is greater than or equal to the key values of any of its children's key values.

* Graph :  stores a collection of items in a nonlinear fashion. Graphs are made up of a finite set of nodes, also known as vertices, and lines that connect them, also known as edges. These are useful for representing real-world systems such as computer networks.

* Trie : also known as a keyword tree, is a data structure that stores strings as data items that can be organized in a visual graph.

* Hash Table : also known as a hash map -- stores a collection of items in an associative array that plots keys to values. A hash table uses a hash function to convert an index into an array of buckets that contain the desired data item.


**Choosing the best data structure**

it depends on : 

1. Supported operations. What functions and operations does the program need?

2. Computational complexity. What level of computational performance is tolerable? For speed, a data structure whose operations execute in time linear to the number of items managed -- using Big O Notation: O(n) -- will be faster than a data structure whose operations execute in time proportional to the square of the number of items managed -- O(n^2).

3. Programming elegance. Are the organization of the data structure and its functional interface easy to use?


***

## LInked lists

**What is a linked list?**

    Linked List is a sequence of links which contains items. Each link contains a connection to another link. Linked list is the second most-used data structure after array.
    Following are the important terms to understand the concept of Linked List:

   1. Link − Each link of a linked list can store a data called an element.
   2. Next − Each link of a linked list contains a link to the next link called Next.
   3. LinkedList − A Linked List contains the connection link to the first link called First.

**Types of Linked List:**

    Simple Linked List − Item navigation is forward only.
    Doubly Linked List − Items can be navigated forward and backward.
    Circular Linked List − Last item contains link of the first element as next and the first element has a link to the last element as previous.

**Basic Operations:**

  Following are the basic operations supported by a list.

   * Insertion − Adds an element at the beginning of the list.
   * Deletion − Deletes an element at the beginning of the list.
   * Display − Displays the complete list.
   * Search − Searches an element using the given key.
   * Delete − Deletes an element using the given key.

**Implementing a Linked List**
 **Advantages of Linked List:**

   1. Because of the chain-like system of linked lists, you can add and remove elements quickly. This also doesn't require reorganizing the data structure unlike arrays or lists. Linear data structures are often easier to implement using linked lists.
   2. Linked lists also don't require a fixed size or initial size due to their chainlike structure.

**Disadvantages of Linked List:**

   1. More memory is required when compared to an array. This is because you need a pointer (which takes up its own memory) to point you to the next element.
   2. Search operations on a linked list are very slow. Unlike an array, you don't have the option of random access.
