#### What is functional programming?
- programming paradigm that treats computation as the evaluation of mathematical functions 
#### What is a pure function and how do we know if something is a pure function?
- function that returns the same result if it is given the same arguments
- also it does not cause any observable side effects
#### What are the benefits of a pure function?
- easier to test
- test pure functions by `given a parameter A -> expect the fucntion to return value B`
#### What is immutability?
- the inability for a data's state to chance after it's created
#### What is Referential transparency?
- if a function consistently gives the same result for the same input
- pure function + immutabale data = referential transparency

---

#### What is a module?
- a split JS program that can be accessed using an import
#### What does the word ‘require’ do?
- it includes external modules that exist in separate files
- loads and cahces JS modeules
#### How do we bring another module into the file the we are working in?
- `require('./<filename>');`
#### What do we have to do to make a module available?
- export the modules and import the features into the script
