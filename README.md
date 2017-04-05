# JS in Depth

## Table of Contents

1. Table of Contents
2. Homework Details
3. JavaScript Questions
4. Node.js Questions
5. React.js Questions
6. Internet/Network questions

## Homework Details

This homework is designed to prepare you for questions you may face during an interview. It should take you no more than 3 hours. It's akin to an open book quiz since you can use the internet to look things up. But first, try going through and seeing how many questions you can answer without using google/stackoverflow/anyOtherInternetSource! And then go back and look up the answers to the ones that stumped you.

## JavaScript Questions

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