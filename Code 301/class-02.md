## Based off the diagram, what happens first, the 'render' or the 'componentDidMount'?
- render happens first, then React updates the DOM and refs, upon which the componentDidMount happens

## What is the very first thing to happen in the lifecycle of React?
- Mounting

## Put the following in order:
1. constructor
2. render
3. React Updates
4. componentDidMount
5. componentWillUnmount

## What does componentDidMount do?
- lets us run React code while the component is already in the DOM
- used to load anything with a network request or intitialize the DOM

---------------------------------------

## What types of things can you pass in the props?
- counter: initial count = 0
  - initializer the component to
  - what you want to component to render like
- display something to the user that has a title and subtitle
  - the application knows that if the props change, it'll re-render that component

## What is the big difference between props and state?
- Props
  - handled outside the component
  - passed into the component  
  - initial count is passed in the Props
  - used for displaying some information isnide a component without hard-coding it 
    - like a variable to a function
- State
  - handled inside the component
  - current count is handled in the State

## When do we re-render our application?
- when we change the state inside of our application

## What are some examples of things that we could store in state?
- updating counter; needs to store a changing value
- used when we need to re-render and update the application based on something the user has done

---------------------------------------
## Things I want to know more about
- How are props and states actively used in React? 
- I understand the differences regarding where a certain component exists during its process of change, but I can't see the practical application and how using either one will affect the result displayed on the screen
