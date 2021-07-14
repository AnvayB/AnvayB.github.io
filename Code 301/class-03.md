### What does .map() return?
- returns an array with the results of the function called on each of the elements of the original array

### If I want to loop through an array and display each value in JSX, how do I do that in React?
``` js
const numbers = [1, 2, 3, 4, 5];
const listItems = numbers.map((numbers) =>
  <li>{numbers}</li>
);

ReactDOM.render(
  <ul>{listItems}</ul>,
  document.getElementById('root')
);
```

### Each list item needs a unique ___
- key

### What is the purpose of a key?
- they help React identify which items have been changed, added or removed

---

### What is the spread operator?
- a JS syntax tool used for adding items to arrays, combining arrays and objects, and spreading an array

### List 4 things that the spread operator can do
- copying an array
- combining objects
- adding an item to a list
- using Math functions

### Give an example of using the spread operator to combine 2 arrays
```js
const myArray = ['A','B','C'];
const yourArray = ['D','E','F'];
const ourArray = [...myArray,...yourArray];
console.log(...ourArray);
```

### Give an example of using the spread operator to add a new item to an array
```js
const letters = [a,b,c];
const moreLetters = [e, f, ...letters];
console.log(moreLetters); // [a,b,c,e,f]
```

### Give an example of using the spread operator to combine 2 objects into one
```js
const objectOne = {hello: 'A'}
const objectTwo = {world: 'B'}
const objectThree = {...objectOne, ...objectTwo, laugh: 'C'}
console.log(objectThree) // Object { hello: "A", world: 'B', laugh: 'C' }
const objectFour = {...objectOne, ...objectTwo, laugh: () => {console.log('C'.repeat(5))}}
objectFour.laugh()
```
---

### In the video, what is the first step that the developer does to pass functions between components?
```js
incrememnt = (name => {
  let ppl = this.state.people.map()
}
```

### In your own words, what does the increment function do?
- it increases the value of the count by 1

### How can you pass a method from a parent component into a child component?
- using props: make a prop that uses the function created in the Parent by writing this.props.`function` to call that function in the Child

### How does the child component invoke a method that was passed to it from a parent component?
- the function passed in the prop can be called with `function()` and passed in the parameters of the Child
