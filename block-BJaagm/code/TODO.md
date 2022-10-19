1. What does thread of execution means in JavaScript?

JavaScript goes line by line through our code and does each line of code.

2. Where the JavaScript code gets executed?

JavaScript code executed in Global Execution Context.

3. What does context means in Global Execution Context?

It is the environment where we execute the code.

4. When do you create a global execution context.

Whenever JS recives the script file it creates the Global Execution Context where all the code get executed line by line.

5. Execution context consists of what all things?

Execution context consists of memory section used to store data and another section where all the computation and execution occurs.

6. What are the different types of execution context?

global execution context and function execution context.

7. When global and function execution context gets created?

when we run script the GEC is being created, it is created once but function execution context created when any function is being run by javascript.

8. Function execution gets created during function execution or while declaring a function.

during function execution  

9. Create a execution context diagram of the following code on your notebook. Take a screenshot/photo and store it in the folder named `img`. Use `![](./img/image-name.png)` to display it here.



```js
var user = "Arya";

function sayHello(){
  return `Hello ${user}`;
}

var userMsg = sayHello(user);
```

<!-- Put your image here -->

![img1](./img/img1.jpeg.jpg)



```js
var marks = 400;
var total = 500;

function getPercentage(amount, totalAmount){
  return (amount * 100) / totalAmount;
}

var percentageMarks = getPercentage(marks, total);
var percentageProfit = getPercentage(400, 200);
```

<!-- Put your image here -->

![img2](./img/img2.jpg)



```js
var age = 21;

function customeMessage(userAge){
  if(userAge > 18){
    return `You are an adult`;
  }else {
    return `You are a kid`;
  }
}

var whoAmI = customeMessage(age);
var whoAmIAgain = customeMessage(12);
```

<!-- Put your image here -->

![](./img/image-name.jpg)