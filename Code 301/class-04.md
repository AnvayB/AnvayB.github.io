### What is a ‘Controlled Component’?
- an input form element whose value is controlled by React due to its rendering being controlled by the form on subsequent user input
### Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.
- 
### How do we target what the user is entering if we have an event handler on an input field?
- the `handleChange` method updates teh React state whenver a keystroke change is made within a certain input field
---

### Why would we use a ternary operator?
- ternary operators serve as a simpler formatting for if/else statements by assigning values into: `condition ? value if true : value if false`
### Rewrite the following statement using a ternary statement 
```js  if(x===y){
 console.log(true);
  } else {
 console.log(false);
  }```
 ```js
 //Answer:
 check = (x===y) ? true : false;
console.log(check);
```

