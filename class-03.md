# HTML Chapter 3: Lists
- `<ol>`: ordered list (1. 2. 3. 4. etc)
- `<ul>`: unordered list (bullet points • • • •)
- `<li>`: list item
- `<dl>`: series of terms and their definitions
- `<dt>`:term being defined
- `<dd>`: definition
- lists can be nested inside each other

# HTML Chapter 13: Boxes
- box dimensions: width, height
- limiting dimensions
  - min-width, min-height
  - max-width, max-height
- each HTML element has its own box according to CSS
- CSS can control the dimensions of the box
  - control the margin, borders, padding, of each box
- you can also hide elements using display and visibility properties
- Block-level boxes can be turned into inline boxes, and vice versa
- legibility of words can be altered by controlling the width (and padding and margin) of boxes containing text and leading
- CSS3 allows for creating image borders and rounded borders

# JS Chapter 2: Basic JS Instructions – Arrays
- arrays store a list of values
- creating an array:
  - `let colors = ["white", "black", "red"];`
  - `let el = document.getElementById("colors");`
  - `el.textContent = colors[0];`
  - Result – Color: white
- values in an array are accessed as though they're in a numbered list, starting with 0
  - `["white", "black", "red"] ==> [0,1,2]`
- accessing and changing values in an array:

![Screen Shot 2021-06-09 at 2 23 31 AM](https://user-images.githubusercontent.com/53208269/121329038-b2485a80-c8c9-11eb-915c-46efc68b3633.png)
`-` from HTML Duckett book, pg 

# JS Chapter 4: Decisions and Loops – Switch statements and on
- covered switch statements and loops in:
  - [Read 02](https://github.com/AnvayB/reading-notes/blob/main/class-02.md)
- Type coercion: JS can convert data types behind the scenes to complete an operation
- Weak typing: JS uses this bc the data type for a value can change
- Strong typing: specifying what data type each variable will be
- Truthy value: treated *as if* they are true
  - almost everything not in the falsy table can be treated as if true
  - can be treated as the number 1
- Falsy value: treated *as if* they are false
  - can be treated as the number 0

![Screen Shot 2021-06-09 at 2 32 16 AM](https://user-images.githubusercontent.com/53208269/121330483-e96b3b80-c8ca-11eb-9878-11f84b45c2cb.png)
`-` from JS Duckett book, pg 167

