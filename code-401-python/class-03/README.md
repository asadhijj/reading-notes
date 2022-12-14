# The Big O

Big O notation is used in Computer Science to describe the performance or complexity of an algorithm. Big O specifically describes the worst-case scenario, and can be used to describe the execution time required or the space used (e.g. in memory or on disk) by an algorithm.

![Basic Big O notation equations](https://d33wubrfki0l68.cloudfront.net/1010f5d18ec531e5f14ab93361391e2d51e7bc82/51941/images/big-o/big-o-graph.svg)


    - An O(1) describes an algorithm that will always execute in the same time (or space) regardless of the size of the input data set.

    - An O(N) describes an algorithm whose performance will grow linearly and in direct proportion to the size of the input data set

    - O(N²) represents an algorithm whose performance is directly proportional to the square of the size of the input data set. This is common with algorithms that involve nested iterations over the data set. Deeper nested iterations will result in O(N³), O(N⁴) etc.

    - O(2^N) denotes an algorithm whose growth doubles with each addition to the input data set. The growth curve of an O(2^N) function is exponential — starting off very shallow, then rising meteorically

    -O(log N). The iterative halving of data sets described in the binary search example produces a growth curve that peaks at the beginning and slowly flattens out as the size of the data sets increase.





## Sources 

[Big 0](https://rob-bell.net/2009/06/a-beginners-guide-to-big-o-notation)
[Part 2](https://medium.com/basecs/whats-a-linked-list-anyway-part-2-131d96f71996)


## Things i want to learn more about 

i really want to learn about the usage of the BIG O with a real python code