1. Convert the function below into different forms of function expression.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}

// Your code goes here
let percentageValue = function percentage(marks, total) {
  return (marks * 100) / total;
}
let percentageValue = (marks, total) => {
  return (marks * 100) / total;
}

```

2. Write Function Declaration or Function Expression next to the function.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}
// Your answer
Function Declaration
```

```js
let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
};
Function Expression
```

```js
let percentage = function (marks, total) {
  return (marks * 100) / total;
};
Function Expression
```

```js
let percentage = (marks, total) => {
  return (marks * 100) / total;
};
Function Expression
```

```js
let percentage = (marks, total) => (marks * 100) / total;
Function Expression
```

3. Why is a function definition an expression in JavaScript? Give one example of function expression.

<!-- Function Expression allows us to create an anonymous function which doesn't have any function name 
let percentage = (marks, total) => (marks * 100) / total; -->

4. Why is a function call an expression in JavaScript?

<!-- A function call expression is used to execute a specified function with the provided arguments.  -->

5. Write VALID and INVALID next to each example below with the reason.

```js
function add(a, b) {
  return a + b;
}

let five = add(2, 3); // Valid
five = add; // Invalid // Here Varible is calling function reference
five = five(10, 11); // Valid
five = function () {
  return 'Hello';
}; // Valid
```

6. What is the difference between function definition and function call? Explain with an example.

<!-- Function definition mean when we write all the code for our function. At that point the function just sits there doing nothing. call is when you tell the JavaScript interpreter to run the code in your function.

function percentage(marks, total) {
  return (marks * 100) / total;
}
Function Declaration
let percentage = (marks, total) => (marks * 100) / total;
Function Expression
 -->

7. What is the similarities between function definition and function call?

<!-- In both function a piece of code is similar, but while calling the function it get executed. -->

8. Is the code below valid or invalid. Explain with reason.

```js
function hello() {
  console.log('Hello World!');
}

hello.user = 'Sam'; // valid
```

9. What is higher order function explain with an example.

 <!-- A Higher-Order function is a function that receives a function as an argument or returns the function as output -->

10. Explain what is callback function. Why you can pass a function inside a function?

<!-- A callback function is a function passed into another function as an argument, which is then invoked inside the outer function to complete some kind of routine or action. -->