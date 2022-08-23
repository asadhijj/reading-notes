# React And Forms 

forms are an essential part of almost every website since the websited requires info from users to enter and this is considered a form, so any type of data that the user enters on the website is some kind of a forms such as login/ sign in forms or user data such as name, national number, birthday .. etc. 
so this is why form are an important topic to cover so we can understand how to make the form on the page interactive with the users.

*** 
## Forms

1. **What is a ‘Controlled Component’?**

An Input form element that is rendered by a React component which controls what happens in that form on subsequent user input but the React state is the singel source of truth.


2. **Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them?** Why.
 it depends on the type of the form and what type of data is required some data must be updated directly like credit card number and some other data should be updated upon submit such as username or password.

3. **How do we target what the user is entering if we have an event handler on an input field?**
after using onChange event handler we can target what the user is entering by using event.target.Value


*** 

## The conditional Ternary operator 


1. **Why would we use a ternary operator?**

to ensure that a specific part of the code only works upon meeting the condition like for example, you can't open your facebook page if you entered the wrong password.

2. **Rewrite the following statement using a ternary statement:**
```javascript
if(x===y){
  console.log(true);
} else {
  console.log(false);
}
```
**as a ternary it can be written as the following :**
```javascript
(x===y)? true : false ;
```

*** 
## Links to external sources 

[Forms](https://reactjs.org/docs/forms.html)
[Ternary Operator](https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff)

***

## Things I want to know more about

i want to learn how is the state used with the form and how the data can be save and tracked.
