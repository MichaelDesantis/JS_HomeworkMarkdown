# JS in Depth

## Table of Contents

1. Table of Contents
2. Homework Details
3. Core JavaScript Questions
4. ES6 Questions
5. Node.js Questions
6. React.js Questions
7. Internet/Network questions

## Homework Details

This homework is designed to prepare you for questions you may face during an interview. It should take you no more than 3 hours. It's akin to an open book quiz since you can use the internet to look things up. But first, try going through and seeing how many questions you can answer without using google/stackoverflow/anyOtherInternetSource! And then go back and look up the answers to the ones that stumped you.

## Core JavaScript Questions

1. What is the difference between `undefined` and `not defined` in JavaScript?
2. What is "Hoisting" in JavaScript?
3. What would be the output of the following code?
```javascript
    var y = 1;
      if (function f(){}) {
        y += typeof f;
      }
     console.log(y);
```
4. What is a "private method"?
5. What is the drawback of creating true private methods in JavaScript?
6. What is a “closure” in JavaScript? Provide an example.
7. Write a mul function which will produce the following outputs when invoked.
```javascript
console.log(mul(2)(3)(4)); // output : 24 
console.log(mul(4)(3)(4)); // output : 48
```
8. How would you empty an array in JavaScript? Provide at least 2 methods of doing so.
9. What will be the output of the following code?
```javascript
var output = (function(x){
    delete x;
    return x;
  })(0);
  
  console.log(output);
```
What about this code?
```javascript
var x = 1;
var output = (function(){
    delete x;
    return x;
  })();
  
  console.log(output);
```
And what about this one?
```javascript
var x = { foo : 1};
var output = (function(){
    delete x.foo;
    return x.foo;
  })();
  
  console.log(output);
```
And finally, what about this one?
```javascript
var Employee = {
  company: 'xyz'
}
var emp1 = Object.create(Employee);
delete emp1.company
console.log(emp1.company);
```
10. What would this code return?
```javascript
var trees = ["xyz","xxxx","test","ryan","apple"];
delete trees[3];
  
  console.log(trees.length);
```
11. What will be the output of the code below?
```javascript
var bar = true;
console.log(bar + 0);   
console.log(bar + "xyz");  
console.log(bar + true);  
console.log(bar + false);   
```
12. What will be the output of the code below?
```javascript
var z = 1, y = z = typeof y;
console.log(y);  
```
13. What would be the output of the code below?
```javascript
 var salary = "1000$";

 (function () {
     console.log("Original salary was " + salary);

     var salary = "5000$";

     console.log("My New Salary " + salary);
 })();

```
14. What is the instanceof operator in JavaScript? What would be the output of the code below?
```javascript
function foo(){ 
  return foo; 
}
new foo() instanceof foo;
```
15. What constitutes a "Primitive" value in Javascript?
16. What is the difference between a reference type variable and a value type variable?
17. How would you describe the difference between class-based inheritance and prototypical inheritance?

## ES6 Questions

1. What is the difference between JavaScript and ECMAScript?
2. What do `const` and `let` do? And when would we use them?
3. How would you describe the difference between `function` and `function*`?
4. When would you NOT use an arrow function in the place of a regular function expression?
5. Refactor the following code to use an ES6 Template Literal.
```javascript
var name = 'Tiger';
var age = 13;

console.log('My cat is named ' + name + ' and is ' + age + ' years old.');
```
6. How would you refactor the following code to use ES6 default parameters?
```javascript
function addTwoNumbers(x, y) {
    x = x || 0;
    y = y || 0;
    return x + y;
}
```
7. What is a "Promise" in ES6? And how many different states do they have?
8. What is a practical use case for Promises? 
9. What is wrong with the following code? And how could it be better?
```javascript
new Promise((resolve, reject) => {  
  throw new Error('error')
}).then(console.log)
```
10. Describe the .fetch() method. What is one disadvantage to using the .fetch() method over existing methods?

## Node.js Questions

1. What is Node.js?
2. What is an "Error-First" Callback?
3. What is the Node.js Event Loop?
4. Why might someone choose to use the Node.js Async single-threaded model over a more traditional multi-threaded model?
5. What is meant by the term "non-blocking I/O"?
6. What is the "memory stack"? And what happens when you exceed it?

## React.js Questions

1. What makes React.js more efficient at updating the DOM?
2. What is the difference between a Logical component and a Pure component?
3. What happens when you call "setState" in React?
4. What is the React method to create a component? Alternatively, how would you accomplish the same thing using ES6 classes?
5. In which React lifecycle event would you make AJAX requests? And why?
6. Why would you use `React.Children.map(props.children, () => )` instead of `props.children.map(() => )`?
7. What is JSX?

## Internet/Network Questions

1. What does TCP/IP stand for?
2. Behind the scenes, how does HTTPS differ from HTTP?
3. Define the general response status code categories.
4. What does DDOS stand for?
5. What is CORS? How does it work?
6. What does REST stand for when we refer it in the context of a "RESTful API"? 

## Resources

https://blog.risingstack.com/node-js-interview-questions-and-answers-2017/
https://www.codementor.io/nihantanu/21-essential-javascript-tech-interview-practice-questions-answers-du107p62z
https://github.com/DrkSephy/es6-cheatsheet
http://career.guru99.com/top-25-interview-questions-on-node-js/
https://tylermcginnis.com/react-interview-questions/
https://hackernoon.com/19-things-i-learnt-reading-the-nodejs-docs-8a2dcc7f307f
http://wesbos.com/arrow-function-no-no/
https://github.com/indy256/Full-stack-Developer-Interview-Questions-and-Answers
https://github.com/arialdomartini/Back-End-Developer-Interview-Questions
https://github.com/h5bp/Front-end-Developer-Interview-Questions