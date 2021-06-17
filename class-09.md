# HTML Chapter 7: Forms
- text input
  - `<input>` is used to create different form controls; type = "text"
- password input
  - typed text is blocked out; type = "password"
- text are
  - multiline text input
- radio button
  - select one option
- checkbox
  - select more than one option
- drop down list
  - select an option from a drop down list
- multiple select box
  - drop down select multiple options from a box
- wherever you want to collect information from visitors, you need a form, inside a form element
  - there are many different types of forms you can use
- information from a form is sent in name-value pairs
- each form control is given a name and the text the user types in or the values of the options they select are sent to the server
- HTML5 introduces new form elements which make it easier for visitors to fill in forms

# HTML Chapter 14: Lists, Tables, and Forms
- in addition to the CSS properties covered in other chapters which work with the contents of all elements, there are several others that are specifically used to control the appearance of lists, tables, and forms
- list markers can be given different appearances using the list-style-type and list-style image properties
- tables cells can have different borders and spacing the different brwosers, but there are properties yuo can use to control them and make them more consistent
- forms are easier to use if the form controls are vertically aligned using CSS
- forms benefit from styles that make them feel more interactive

# JS Chapter 6: Events
![Image 6-17-21 at 2 59 AM](https://user-images.githubusercontent.com/53208269/122375305-f4038180-cf17-11eb-82db-f5e63abdbdcb.jpg)
![Image 6-17-21 at 3 00 AM](https://user-images.githubusercontent.com/53208269/122375536-27dea700-cf18-11eb-8305-7fdc46337621.jpg)
`-` from Duckett JS book, pg 246-247
- events are the browser's way of indicating when something has happened (ex: page has finished loading or button has been clicked)
- binding is the process of stating which event you are waiting to happen, and which element you are waiting for that event to happen upon
- when an event occurs on an element, it can trigger a JS function.
  - when this function then changes the web page is some way, it feels interactive bc it has responded to the user
- you can use event delegation to monitor for events that happen on all of the children of all element
- the most commonly used events are W3C DOM events 
  - although there are others in the HTML5 specification as well as browser-specific events
