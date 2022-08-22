# Read Class 3
- **Topics included :**
1. Map()
2. Spread operator
3. Passing functions to components

***
## Map()
---
The map function is an important loop tool that helps making the process accessing data easier and faster which is very important to be able to make the work cleaner and more efficient.

1. **What does .map() return?** a loop function
2. **If I want to loop through an array and display each value in JSX, how do I do that in React?** using the map()     function returning <li> element for each item and then assigning the resulting array to a list of items, then including the whole list into <ul>.
3. **Each list item needs a unique** ____.key
4. **What is the purpose of a key?** to help react identify which items have changed or added or removed.

***

## Spread Operator
---
Spread OPerator is also an important syntax since it allows controlling Arrays and objects by adding items to them or even combining them in quick way.

1. What is the spread operator? a quick syntax for adding items into arrays and also combining arrays or objects, and  also spreading arrays out into a function's argument.
2. List 4 things that the spread operator can do.
Copying an array
Concatenating or combining arrays
Using Math functions
Using an array as arguments

3. Give an example of using the spread operator to combine two arrays.
```javascript
const smallNumbers = [1,2,3,4,5]
const bigNumbers = [100,200,300,400,500];
const combined = [...smallNumbers,...bigNumbers]
console.log(...combined);
```

4. Give an example of using the spread operator to add a new item to an array.
```javascript
const numbers = [1,2,3]
const addinNumbers = [4,5,6, ...numbers]
console.log(addinNumbers) 
```

5. Give an example of using the spread operator to combine two objects into one.
```javascript
const first = {name: "Asad"}
const last = {surname : "Hijawi"}

const fullName = {...first,...last}
console.log(fullName);
```

***

## Passing Functions to Components
---
This is a very important topic in React since it allows the developer to make the code interactive with user by sending and passing data to it which makes the process fluid.

1. In the video, what is the first step that the developer does to pass functions between components? 
create a function whereever the state is (parent).
2. In your own words, what does the increment function do? 
it is a function that increases the count in the object passed to it.

3. How can you pass a method from a parent component into a child component?
we pass it as a prop into the child component.
4.How does the child component invoke a method that was passed to it from a parent component?
 the method gets called in the child component which will change the state causing a rerender that is gonna pass down and props the new value of count.

***
* Links to resources :
1. [React Docs - list and keys](https://reactjs.org/docs/lists-and-keys.html)
2. [The spread operator](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)
3. [Passing Functions](https://www.youtube.com/watch?v=c05OL7XbwXU)

***

## Things I want to know more about
---
i am curious about how can user interactive data be saved in the memory using React

