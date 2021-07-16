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

### What does it mean to build a ‘static’ version of your application?

### Once you have a static application, what do you need to add?

### What are the three questions you can ask to determine if something is state?

### How can you identify where state needs to live?
