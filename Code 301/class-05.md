### How would you break a mock into a component heirarchy?
- separate each section of the UI
- For example: 

![Screen Shot 2021-07-16 at 12 15 18 AM](https://user-images.githubusercontent.com/53208269/125907740-5a6aad73-3fb5-4c8a-b8c4-7ae357927758.png)

from [Thinking in React](https://reactjs.org/docs/thinking-in-react.html)

  - FilterableProductTable(orange): entire table/object
  - SearchBar(blue): takes in user input about products
  - ProductTable(green): categorizes data based on 'Name' and 'Price' on an x-axis and 'Sporting Goods' and 'Electronics' on the y-axis
  - ProductCategoryRow(turquoise): emboldened heading for the y-axis categories
  - ProductRow(red): displays row for each product

### What is the single responsibility principle and how does it apply to components?
- a component should do one and only one thing
  - reduces risks of a component being reused for another purpose anf potentially breaking the code

### What does it mean to build a ‘static’ version of your application?
- it means building a version that takes the app's data model and UI but doesn't implement any interactivity (no state)

### Once you have a static application, what do you need to add?
- an instance property to the constructor to reflect the initial state of your application

### What are the three questions you can ask to determine if something is state?
- Is it passed in from a parent via props? 
  - If so, it probably isn't state.
- Does it remain unchanged over time?
  - If so, it probably isn't state.
- Can you compute it based on any state or props in your component?
  - If so, it isn't state.

### How can you identify where state needs to live?
- the state needs to live in the – as per the example – `FilterableProductTable` because 
  - the `ProductTable`needs to filter the product list based on state and the `SearchBar` needs to display the search text and checked state
  - and the common component betweem the 2 is `FilterableProductTable`
