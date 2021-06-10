# HTML Chapter 4: Links
### writing links: 
- Linking to other sites: `<a href = "http://www.link.com">Link Title</a>`
- Linking to other pages on same site: `<a href = "index.html">Home<a/>`
- Email links: `<a href = "mailto:jon@example.com">Email Jon</a>`
- Opening links in new window: `<a href = "http://www.link.com" target = "_blank">`
- Linking to parts of same page: use relative links instead of qualified URLs
```
<a href = "#home">Homepage</a>
...
<h2 id = "home">Homepage</a>
```

# HTML Chapter 15: Layout
- `<div>` elements are used as contiaing elements to group sections of a page tovether
- browsers display pages in normal flow unless relative/absolute/fized positioning has been specified
- the `float` property moves content to the left or right of the page and can be used to create multi-column layouts
  - floated items require a defined width
- designers keep pages within 960-1000 px wide, and indicate what the site is about within the top 600 px
  - this demonstrates its relevance without the user having to scroll
- grids help create professional and flexible designs
- CSS frameworks provide rules for common tasks
- you can include multiple CSS files in one page

# JS Chapter 3: Functions, Methods, and Objects – Part 1
- Functions let you group a series of statements together and perform a specific task 
- If different parts of the script need the same task, you can reuse the same function, rather that writing a new series of the same statements
- Declaring a function:
```
  function sayHello() {
    document.write('Hello!');
  }
```
- Calling a function: `sayHello();`
```
  function calcArea(width, height) {
    let area = width * height;
    return area;
  }
  let wall1 = calcArea(3,5);
```
```
function getSize(width, height, depth) {
  let area = width * height;
  let volume = area * depth
  let sizes = [area, volume];
  return sizes;
}
let area1 = getSize(3,2,3)[0];
let volume1 = getSize(3,2,3)[1];
```

# 6 Reasons for Pair Programming
1. 
