# JS Chapter 10: Error Handling & Debugging
- if you understand exectution contexts (2 stages) and stacks, you are more likely to find the error in your code.
- debudding is the process of finding errors
  - involves the process of deduction
- the console helps narrow down the area in whic is error is located, so you can try to find that exact error 
  - which line (and sometimes which column of text) it's on
- JS has 7 different types of errors
  - Syntax error: syntax is not correct
   ```js 
   document.write("Howdy!');
   ```
  - Reference error: variable does not exist
  ```js 
   let width = 4;
   let area = width * height;
   //or
   document.write(getArea());
   ```
   - Eval error: incorrect use of `eval(): evaluates text through the interpreter` function
   - URI error: incorrect use fo uri functions, these characters not allowed: `/ ? & # : ; `
   ```js 
   decodeURI('http://bbc/com/news/php?a=1');
   ```
   - Type error: value is unexpected data type, method doesn't exist
   ```js 
   document.WRITE("Oops!");
   ```
   - Range error: number outside of range
   ```js 
   let array = new Array(-1);
   ```
   - Error: generic error object, template/prototype for all other error objects
