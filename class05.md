# Thinking in React 

learning how React thinks and processes things gives the developer a better understanding of how they should deal with React and makes you get a better thought of hoow to build the app you want to build

***
## Thinking in React 

1. **What is the single responsibility principle and how does it apply to components?**
it is a priniciple that stated that a component should ideally do one thing only, if its to grow it should be broken down into smaller subcomponents.

2. **What does it mean to build a ‘static’ version of your application?**
it is a version of the the app that is made to render the data but its not interactive at all because you build a component that reuses other components and pass data using props, which pass data from parent component to a child component and the data that it passes is static and not iteractive.

3. **Once you have a static application, what do you need to add?**

you need to make the app interactive by adding state to it which allow the data to be updated through interactions.

4. **What are the three questions you can ask to determine if something is state?**

    1. Is it passed in from a parent via props? If so, it probably isn’t state.
    2. Does it remain unchanged over time? If so, it probably isn’t state.
    3. Can you compute it based on any other state or props in your component? If so, it isn’t state.


5. **How can you identify where state needs to live?**
we can identify where the state live by following the next steps :

    1. Identify every component that renders something based on that state.
    2. Find a common owner component (a single component above all the components that need the state in the hierarchy).
    3. Either the common owner or another component higher up in the hierarchy should own the state.
    4. If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add 5. it somewhere in the hierarchy above the common owner component.

***

## Higher Order Function

these functions are important because it allow to us abstract over actions not only values

1. **What is a “higher-order function”?**

Functions that operate on other functions, either by taking them as arguments or by returning them.

2. **Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?**

the second line takes 2 functions to compare between, since :
definning the 
```javascript
function greaterThan(n) {
  return m => m > n;
}
let greaterThan10 = greaterThan(10);
console.log(greaterThan10(11));
// Explaination
let greaterThan10 = greaterThan(10); // in this line a variable greaterThan10 is assigned witht the function greaterThan passing the value 10 for n
console.log(greaterThan10(11)); // and in this line the function is called passing 10 as 'n' and then the value 11 as the 'm' parameter.

 return m => m > n; // so basically this second line takes 2 functions and compares between the parameters passed since we have a normal function and an arrow function.
```

3. **Explain how either map or reduce operates, with regards to higher-order functions.**

the map method transforms through all the array elements applying a function that building a new araay of the same length and returns the value of the new array, meanwhile the reduce operator works by repeatedely taking an array element and combine it with the current value like for example summing elements, it takes a single element and adds it for the current value of the summation doing the same process for each element.


***
## Links to external sources 
[Thinking React](https://reactjs.org/docs/thinking-in-react.html)
[Higher Order Functions](https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK)

***

## Things I want to know more about
hoe to use these operators inside a real application.






