# OOP Part02

## Software Design Patterns 

A design pattern is only a description or template for how to solve a problem! that can be used in many different situations

In the case of object-oriented programming paradigm, design patterns are generally aimed at solving the problems of object generation and communication, rather than the larger scale problems of overall software architecture.

**There is 3 major types of design patterns:**

1. Creational Patterns: 
    Creational patterns provide ways to instantiate single or groups of objects. Making it easier to create objects in a way that suits the situation.

Some Creational Patterns:
    * Factory Method
    * Singleton
    * Abstract Factory

2. Structural Patterns:
    Structural patterns provide a manner to define relationships between classes or objects. Making it easier for these entities to work together.

Some Structural Patterns:
    * Facade
    * Adapter
    * Decorator

3. Behavioral Patterns:
    Behavioral patterns define manners of communication between classes and objects. Making it easier and more flexible for these entities to communicate.

Some Behavioral Patterns:
   * Observer.
   * Mediator
   * Chain of Responsibility


***

## Risk Analysis

The probability of any unwanted incident is defined as Risk.
 In Software Testing, risk analysis is the process of identifying the risks in applications or software that you built and prioritizing them to test. After that, the process of assigning the level of risk is done. The categorization of the risks takes place, hence, the impact of the risk is calculated

**Why use Risk Analysis?**

In any software, using risk analysis at the beginning of a project highlights the potential problem areas. After knowing about the risk areas, it helps the developers and managers to mitigate the risks. When a test plan has been created, risks involved in testing the product are to be taken into consideration along with the possibility of the damage they may cause to your software along with solutions.

**Possible Risks**

    * Use of new hardware
    * Use of new technology
    * Use of new automation tool
    * The sequence of code
    * Availability of test resources for the application


**Risks that are unavoidable**

    * The time that you allocated for testing

    * A defect leakage due to the complexity or size of the application

    * Urgency from the clients to deliver the project

    * Incomplete requirements


**Risk magnitude indicators**

* High: means the effect of the risk would be very high and non-tolerable. The company might face loss.

* Medium: it is tolerable but not desirable. The company may suffer financially but there is a limited risk.

* Low: it is tolerable. There lies little or no external exposure or no financial loss.


**Risk Identification**

   1. Business Risks: This risk is the most common risk associated with our topic. It is the risk that may come from your company or your customer, not from your project.

   2. Testing Risks: You should be well acquainted with the platform you are working on, along with the software testing tools being used.

   3. Premature Release Risk: a fair amount of knowledge to analyze the risk associated with releasing unsatisfactory or untested software is required

   4. Software Risks: You should be well versed with the risks associated with the software development process.


**Risk Assessment**

![Risk Assessment](https://d1jnx9ba8s6j9r.cloudfront.net/blog/wp-content/uploads/2019/08/Picture1-528x290.png)


There are three perspectives of Risk Assessment:

* Effect -> To assess risk by Effect. In case you identify a condition, event or action and try to determine its impact.

* Cause -> To assess risk by Cause is opposite of by Effect. Initialize scanning the problem and reach to the point that could be the most probable reason behind that.

* Likelihood -> To assess risk by Likelihood is to say that there is a probability that a requirement won’t be satisfied.



***

## Dependency Injection

In software engineering, dependency injection is a technique whereby one object (or static method) supplies the dependencies of another object. A dependency is an object that can be used (a service).

dependency injection is transferring the task of creating the object to someone else and directly using the dependency 

**There are basically three types of dependency injection:**

    * constructor injection: the dependencies are provided through a class constructor.
    * setter injection: the client exposes a setter method that the injector uses to inject the dependency.
    * interface injection: the dependency provides an injector method that will inject the dependency into any client   passed to it. Clients must implement an interface that exposes a setter method that accepts the dependency.

**So now its the dependency injection’s responsibility to:**

   * Create the objects
   * Know which classes require those objects
   * And provide them all those objects


**Inversion of control —the concept behind DI**

This states that a class should not configure its dependencies statically but should be configured by some other class from outside.

It is the fifth principle of S.O.L.I.D — the five basic principles of object-oriented programming and design by Uncle Bob — which states that a class should depend on abstraction and not upon concretions (in simple terms, hard-coded).

According to the principles, a class should concentrate on fulfilling its responsibilities and not on creating objects that it requires to fulfill those responsibilities. And that’s where dependency injection comes into play: it provides the class with the required objects.


**Benefits of using DI**

   1. Helps in Unit testing.
   2. Boiler plate code is reduced, as initializing of dependencies is done by the injector component.
   3. Extending the application becomes easier.
   4. Helps to enable loose coupling, which is important in application programming.

**Disadvantages of DI**

   1. It’s a bit complex to learn, and if overused can lead to management issues and other problems.
   2. Many compile time errors are pushed to run-time.
   3. Dependency injection frameworks are implemented with reflection or dynamic programming. This can hinder use of IDE automation, such as “find references”, “show call hierarchy” and safe refactoring.


***

## Sources 

[Software Design Patterns](https://medium.com/@Mahmoud_Zalt/software-design-patterns-simplified-8a72232d52b1)

[Risk Analysis](https://www.edureka.co/blog/risk-analysis-in-software-testing/)

[Dependency Injection](https://www.freecodecamp.org/news/a-quick-intro-to-dependency-injection-what-it-is-and-when-to-use-it-7578c84fa88f/)


***

## Things i want to learn more about 

1. the implemntation of design patterns

2. Dependency Injection usage cases and how to implemnt it in a real project