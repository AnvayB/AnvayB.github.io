#### What is a ‘call’?
- function invocation
#### How many ‘calls’ can happen at once?
- 1 at a time
#### What does LIFO mean?
- Last In, First Out
#### Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.
![Screen Shot 2021-07-23 at 8 33 30 AM](https://user-images.githubusercontent.com/53208269/126805834-c920e7a0-6232-4e30-aabb-f5178757fee0.png)
```js
function firstFunction(){
  throw new Error('Stack Trace Error');
}

function secondFunction(){
  firstFunction();
}

function thirdFunction(){
  secondFunction();
}

thirdFunction();
```
#### What causes a Stack Overflow?
- when there is a recursive function without an exit/break point
---

#### What is a ‘refrence error’?
- trying to use a variable that hasn't been declared yet
#### What is a ‘syntax error’?
- something that cannot be parsed in terms of syntax of the code
#### What is a ‘range error’?
- trying to manipulate an object with some kind of length and it is given an invalid length (negative)
#### What is a ‘type error’?
- when the types (number, strings, etc) being used or accessed are incompatible 
#### What is a breakpoint?
- when running a debugger, the breakpoint is the line where you want the code to break or stop
#### What does the word ‘debugger’ do in your code?
- the debugger allows you to see what is happening/changing in your data at each line progression 
