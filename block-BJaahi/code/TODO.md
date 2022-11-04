For the given code below:

- re-write the code in ways that system will understand

For Example:

1.

```js
var username = 'Arya';
let brothers = ['John', 'Ryan', 'Bran'];

console.log(username, brothers[0]);

function sayHello(name) {
  return `Hello ${name}`;
}

let message = sayHello(username);
var nextMessage = sayHello('Test');
```

<!-- Answer -->

```js
// Declaration Phase
var username = undefined;
let brothers;

function sayHello(name) {
  return `Hello ${name}`;
}

let message;
var nextMessage = undefined;

// Execution Phase

username = 'Arya';
brothers = ['John', 'Ryan', 'Bran'];

console.log(username, brothers[0]);

message = sayHello(username);
nextMessage = sayHello('Test');
```

2.

```js
console.log(username, number);

var username = 'Arya';
let number = 21;

function sayHello(name) {
  return `Hello ${name}`;
}

let message = sayHello(username);
var nextMessage = sayHello('Test');
```

<!-- Answer -->

```js
// Declaration Phase
var username = undefined;
let number;

function sayHello(name) {
  return `Hello ${name}`;
}
let message;
var nextMessage = undefined;

// Execution Phase
console.log(Arya, `not defined`);


```

3.

```js
console.log(username, number);
let username = 'Arya';
let number = 21;

let sayHello = function (name) {
  return `Hello ${name}`;
};

let message = sayHello(username);
var nextMessage = sayHello('Test');
```

<!-- Answer -->

```js
// declaration phase
let username;
let number;

let sayHello;
let message;
var nextMessage = undefined;

// execution phase
console.log(undefined, undefined);
```

4.

```js
let username = 'Arya';
console.log(username, number);

let number = 21;
let message = sayHello(username);

let sayHello = function (name) {
  return `Hello ${name}`;
};

var nextMessage = sayHello('Test');
```

<!-- Answer -->

```js
// declaration phase
let username;
let number;
let message;
let sayHello;

var nextMessage = undefined;

// execution phase
console.log(Arya, undefined);
```

5.

```js
console.log(name);
console.log(age);
var name = 'Lydia';
let age = 21;
```

<!-- Answer -->

```js
// Declaration phase

var name = undefined;
let age;

// Execution phase
Lyndia
age not defined
```

6.

```js
function sayHi(name) {
  console.log(name);
  console.log(age);
  var name = 'Lydia';
  let age = 21;
}

sayHi();
```

<!-- Answer -->

```js
// Declaration phase
function sayHi(name) {
  console.log(name);
  console.log(age);
  var name = 'Lydia';
  let age = 21;
}
// Execution Phase
// Declaration Phase of sayHi
var name = undefined;
let age;

// Execution Phase of sayHi
undefined
age is not defined

```

7.

```js
sayHi();
function sayHi(name) {
  console.log(name);
  // console.log(age);
  var name = 'Lydia';
  let age = 21;
}
```

<!-- Answer -->

```js
// Declaration Phase
function sayHi(name) {
  console.log(name);
  console.log(age);
  var name = 'Lydia';
  let age = 21;
}
// Execution Phase
sayHi();
// Declaration Phase of sayHi
var name = undefined;
let age;
// Execution Phase of sayHi
console.log(undefined)
Cannot access 'age' before initialization

```

8.

```js
sayHi();
let sayHi = function sayHi(name) {
  console.log(name);
  console.log(age);
  var name = 'Lydia';
  let age = 21;
};
```

<!-- Answer -->

```js
// Declaration Phase
let sayHi;
var name = undefined;
let age;

// Execution phase
sayHi is not defined
```

9.

```js
let num1 = 21;
console.log(sum);
var sum = num1 + num2;
let num2 = 30;
```

<!-- Answer -->

```js
// Declaration Phase
let num1;
var sum;
let num2;
// Execution phase
num1 = 21;
console.log(undefined)
```

10.

```js
var num1 = 21;

let sum2 = addAgain(num1, num2, 4, 5, 6);

let add = (a, b, c, d, e) => {
  return a + b + c + d + e;
};
function addAgain(a, b) {
  return a + b;
}
let num2 = 200;

let sum = add(num1, num2, 4, 5, 6);
```

<!-- Answer -->

```js
// Declaration Phase
var num1 = undefined;
let sum2;
let add;
function addAgian(a, b) {
  return a + b;
}
let num2;
let sum;

//Execution Phase
num1 = 21;
sum2 =  addAgain(num1, num2, 4, 5, 6);
add = (a, b, c, d, e) => {
  return a + b + c + d + e;
};num2 is not defined

```

11.

```js
function test(a) {
  let num1 = 21;
  return add(a, num1);
}

let sum = test(100);

let add = (a, b) => {
  return a + b;
};
```

<!-- Answer -->

```js
// Declartion Phase
function test(a) {
  let num1 = 21;
  return add(a, num1);
}
let sum;
let add;
// Execution Phase
sum = test(100);
// declaration phase of test
let a;
let num1;
// execution phase of test
a = 100;
num1 = 21;
add is not defined
```

12.

```js
function test(a) {
  let num1 = 21;
  return add(a, num1);
}

let sum = test(100);

function add(a, b) {
  return a + b;
}
```

<!-- Answer -->

```js
// Declaration Phase
function test(a) {
  let num1 = 21;
  return add(a, num1);
}
let sum;
function add(a, b) {
  return a + b;
}
//Execution phase
sum = test(100)
// Declaration Phase of test
let num1;
//Execution phase
num1 = 21;
calling function add;
// Declaration Phase of add
let a;
let b;
// Execution Phase of add
a = 100;
b = 21;
return value 121 will be saved to sum;

```
