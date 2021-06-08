# HTML Chapter 2: Text
1. Headings
- HTML has 6 levels of headings: h1, h2, h3, h4, h5, h6
  - `<h1>`: main headings
  - `<h2>`: subheadings
  - `<h3>`, etc: smaller subheadings
2. `<p>`: paragraph
3. `<b>`: bold
4. `<i>`: italics
5. `<sup>`: superscript
6. `<sub>`: subscript
7. `<br />`: line break --> new line
8. `<hr />`: break between lines --> horizontal line
9. `<strong>`: content has strong importance
10. `<em>`: content has emphasis
11. `<blockquote>`: indent the contents of a large quote
12. `<q> </q>`: quotation marks
13. `<abbr>`: add abbreviations 
14. `<acronym title = "------">`: hold acronyms
15. `<cite>`: referencing citations
16. `<dfn>`: indicate definitions of terms
17. `<address>`: contain link of contact info (of author of page)
18. `<del>`: indicate content has been deleted
19. `<ins>`: indicate content has been inserted (in place of deletion)
20. `<s>`: strikethrough
21. All these tags serve to provide semantic reference for other viewers of your code

# HTML Chapter 10: Introducing CSS
- Thinking Inside the Box
- CSS associates style rules with HTML elements
- CSS rules:
  - selector { declaration; }
    - p { color: blue; }
  - property { value; }
    - h1, h2, h3 { font-family: Arial; color: yellow; }
1. External CSS
- `<link href="css/styles.css" type = "text/css" rel = "stylesheet" />`
  - href: path to CSS file
  - type: type of c=document being linked to
  - rel: relationship between HTML page and CSS file
2. Internal CSS
- `<style type = "text/css"> </style>`
- CSS rules within an HTML page
3. CSS selectors:

![Screen Shot 2021-06-08 at 1 35 09 AM](https://user-images.githubusercontent.com/53208269/121152095-c4f35e80-c7f9-11eb-9a6c-eb112e48dc5c.png)
`-`Duckett HTML book, pg 238

# JS Chapter 2: Basic JS Instructions
- script is a series of instructions
- variables: var quantity; quantity = 3;  
  - store temporary peices of info (data) that are used later in the script
- Arrays: store a set of related data 
- JS variables distinguish between numbers, strings, and Boolean values
- Expressions rely on operations to calculate values and evaluate into a single value
- Arithmetic Operations:

![Screen Shot 2021-06-08 at 1 49 13 AM](https://user-images.githubusercontent.com/53208269/121154322-bb6af600-c7fb-11eb-9e8e-64e825adf9f8.png)
`-` Duckett JS book, pg 76

# JS Chapter 4: Decisions and Loops
- Comparisons
-  used for comparing numbers or expressions
  - == - is equal to
  - != - is not equal to
  - === - strict equal to
  - !== - strict not equal to
  - `>` - greater than
  - `<` - less than
  - `>=` - greater than or equal to
  - `<=` - less than or equal to
- Logical Operators
  - && - logical AND
  - || - logical OR
  - ! - logical NOT
- If/Else Statements
  - if (score >= 85)
    - { congratulate; }
  - else {
    - { encourage; }
- Switch statements
  - faster than if/else
  - finds the case that matches the input and runs that code
  - otherwise, runs the default code
  - allows for more options than if/else
  
![Screen Shot 2021-06-08 at 2 03 21 AM](https://user-images.githubusercontent.com/53208269/121156628-b5761480-c7fd-11eb-8a73-e2b06bc96709.png)
 `-` Duckett JS book, pg 164 
 
 - Data Types in JS
   - string : Text
   - number : Number
   - Boolean : T/F
   - null : Empty value
   - undefined: variable has been declared but not yet assigned a value

- Loops
  - for: run a code a specific number of times
  - while: run a code until a certain condition is met
  - do while: similar to ^; will always run the code inside the {} at least once, even if the condition evaluates to `false`
  - Loop counters
    - Initialization: var i = 0;
    - Condition: i < 10;
    - Update: i++

![Screen Shot 2021-06-08 at 2 10 26 AM](https://user-images.githubusercontent.com/53208269/121157794-b2c7ef00-c7fe-11eb-8b38-552c67672b15.png)

`-` Dockett JS book, pgs 172-173
