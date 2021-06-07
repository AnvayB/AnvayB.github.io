# HTML Chapter 1: Structure
1. Tags act as containers of page information
  - html: HTML code 
  - body: main browser window
  - h1, h2: subheadings of decreasing size
  - p: paragraph of text
2. Attributes provide information about the contents of an element using a *name* = "*value*" format
  - Ex: img src = "*http link*"
  - Ex: p *lang* = "*en-us*" --> determines the language of the page
3. Body, Head, Title
  - Before the body tag, there are head & title tags
  - Head: contains info about the page
    - essentially just the title section
  - Title: references what text will appear as the title of the window or browser tab
 4. Summary
  - HTML pages are text docs
  - HTML uses tags (angle brackets) to give the info they surround special meaning
  - tags are referred to as elements
  - tags often come in pairs; closing tag has a forward slash after the first angle bracket
  - opening tags can contain attributes, which tell us about the content of the element
  - attributes require a *name* and *value*

# HTML Chapter 8: Extra Markup
1. !DOCTYPE html: tells browser which version of HTML (HTML5) we're using
  - different tag content for older versions
2. Comments in HTML
  - used to tell yourself and others what a certain block of code does, or where you got it from
3. id Attribute
  - aka global attribute
  - can be used to reference certain elements when styling page in CSS
 4. class Attribute
  - similar to id
  - but used to reference several elements when styling page in CSS
 5. Block Elements
  - elements that will start on a new line
    - Ex: h1, p, li, ul
 6. Inline Elements
  - elements that will continue to appear on the same line as others
    - Ex: a, b, em, img
 7. Grouping Text & Elements in a Block
  - div allows you to group elements into 1 block-level box


# HTML Chapter 17: HTML 5 Layout
1. Headers & Footers
  - header, footer
    - main header/footer that appears at top/bottom of each page
2. Navigation
  - nav
    - contains major navigational blocks directing to certain pages on the site
3. Articles
  - article
    - acts as a container for any standalone length of code
4. Asides
  - when used inside *article* element, contains info related but not essential to *article*

# HTML Chapter 18: Process & Design
- Who is the site for?
  - target audience? demographic? location? 
  - what is their attitude when viewing the site?
  - what info will the users need?
  - how often will people visit the site?
  - test the site's functionalities by using the website through the eyes of various (fictional) users
- Why are people visiting the site? What are they trying to achieve?
  - information? shopping? recreation?
- Use site maps to determine how various pages should be grouped 
![Screen Shot 2021-06-07 at 3 44 42 AM](https://user-images.githubusercontent.com/53208269/121003717-b39b4b00-c742-11eb-82bd-301a2f70359c.png)
- use wireframes to create hierarchy of info and sketch how info should be viewed
![Screen Shot 2021-06-07 at 3 46 16 AM](https://user-images.githubusercontent.com/53208269/121003925-eb09f780-c742-11eb-9529-3173eff11b2e.png)
- Grouping helps organize info so that user can comprehend the site easily
![Screen Shot 2021-06-07 at 3 47 48 AM](https://user-images.githubusercontent.com/53208269/121004116-2278a400-c743-11eb-813e-9789761bc225.png)


# JS Chapter 1: The ABCs of Programming
- What is a script?
  - series of instructions that the computer executes to complete a task
  - when the script runs, only a subset of all instructions are being used
  - computers interpret commands more technically than humans, so scripts need to be written in the most basic form to ensure that each step is completed
- How do computers fit in the world?
  - computers use data to create models of the world
  - models use objects: represent physical things using properties --> perform tasks --> trigger events
    - when a certain event occurs, another event can be triggered as a result
  - HTML markup is used to create models of web pages
  - web pages are made interactive by using the browser's model of the web page
- How is script written for a web page?
  - JS code should have its own file, and be referenced in the HTML code (same for CSS files)
  - the HTML *script* element is used to tell the browser to load the JS file (similar to *link* to load a CSS file)
  - viewing the source code of a page shows that the JS hasn't changed the HTML code bc the script works with the web page model
