# Understanding the Problem Domain
- hardest part about writing code
  - learning new tech
  - naming things
  - testing code
  - debugging
  - making software maintainable
- Problem Domain: info that defines the probelm and constrains the solution
- make PD easier by cutting out cases and narrowing focus to specific part of the problem
  - take part of the problem and fully understand it before expanding your reach to other problems

# JS Chapter 3: Object Literals
- Objects group together a set of variables and functions to create a model of something you'd recognize from the real outside world
- variables and functions take new names
- properties: variables; methods: functions
- creating an object:
``` javascript
var hotel {
  name: 'Quay',
  rooms: 40,
  booked: 25,
  checkAvailability: function() {
    return this.rooms - this.booked;
  }
};
```
- "this" keywod is used to indicate that it is using the **rooms** and **booked** properties of ***this*** object
- accessing an object:
``` javascript
var hotelName = hotel.name;
var roomsFree = hotel.checkAvailability();
```
# JS Chapter 5: Document Object Model
- the browser represents the page using a DOM tree
- DOM trees have 4 types of nodes:
  - document nodes
  - element nodes
  - attribute nodes
  - text nodes
- you can select element nodes by their id or class attributes, by tag name, or using CSS selector syntax
- whenever a DOM quer can return more than 1 node, it will always return a NodeList
- from an element node, you can access and update its content using properties such as textContent and innerHTML or using DOM manipulation techniques
- an element node can contain multiple text nodes and child elements that are siblings of each other
- in older browsers, implementation of DOM is inconsistent (and a popular reason for using jQuery)
- browsers offer tools for viewing the DOM tree
