# Domain Modeling
- process of creating a concpetual model in code for a specific problem
  - describes various entities, their attribtues and behaviors, and the constraints that govern the problem domain
    - entity that stores data in properties and encapsulates behaviors in methods is referred to as an Object-Oriented model
  - a well articulated domain model can verify and validate the understanding of a specific problem among various stakeholders
  - communcation tool: it defines a vocabulary that can be used within and between both technical and business teams
- tips for building domain models
  1. when modeling a single entity that'll have many instances, build self-contained objects with the same attributes and behaviors
  2. model its attributes with a constructor function that defines and initializes properties
  3. model its begaviors with small methods that focus on doing 1 job well
  4. create instances using the `new` keyboard followed by a call to a constructor function
  5. store the newly created object in a variable so you can access its proerties and methods from **outside**
  6. use the `this` variable within methods so you can access the object's properties andmethods from **inside**

# HTML Chapter 6: Tables
- table represents information in a grid format
``` html
<table>  <!--create a table-->
  <tr>  <!-- start table row-->
    <th> <!-- table heading-->
      <td> <!--insert table data-->
      </td>
  </th>
  </tr>
</table>
```
- you can make cells of a table span more than 1 row or column using the `rowspan` and `colspan` attributes
- for long tables, you can split the table into a `<thead>, <tbody>, and <tfoot>`
# JS Chapter 3: Functions, Methods, Objects
- functions allow you to group a set of related statements together that represent a single task
- functions can take parameters (information required to do their job) and may return a value
- an object is a series of variables and functions that represent something from the world around you
- in an object, variables are known as properties of the the object
  - functions are knows an methods of the object
- web browsers implement objects that represent both the browser window and the document loaded into the browser window
- JS also has internal built-in objects such as `String, Number, Math`, and `Date`
  - their properties and methods offer functionality that helps to write scripts
- arrays and objects can be used to create complex data sets 
  -  both can contain the other
