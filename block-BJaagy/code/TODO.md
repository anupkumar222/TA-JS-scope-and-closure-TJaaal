1. Create a function by your choice that accepts a callback function.

2. Create a function by you choice that returns a function reference.

3. Create a higher order function called `map` that takes two inputs:
   - An array of numbers/string/boolean etc
   - A 'callback' function - a function that is applied to each element of the array (inside of the function 'map')

Have `map` return a new array filled with values that are the result of the 'callback' function on each element of the input array.

```js
// Your code goes here
function multiplyArrayByN(arr, cb) {
  let finalArr = [];
  for (let elm of arr) {
    finalArr.push(cb(elm));
  }
  return finalArr;
} 
// Test Your Code
function multiplyByTwo(n) {
  return n * 2;
}
let mapArr = multiplyArrayByN([1, 2, 3, 4, 5], multiplyByTwo); //-> [2,4,6,8,10]
multiplyByTwo(1); //-> 2
multiplyByTwo(2); //-> 4
let multipleTwo = multiplyArrayByN([1], multiplyByTwo);
let multipleWithTwo = multiplyArrayByN([2], multiplyByTwo);
```

4. Create a higher-order function called `forEach` that takes an array and a callback, and runs the callback on each element of the array. `forEach` does not return anything.

```js
function forEach(str, cb) {
  return letters.forEach(letter => {
    cb(letter);
  })
 
}

// Test Your Code
let alphabet = '';
let letters = ['a', 'b', 'c', 'd'];

function alpha() {
forEach(letters, function (char) {
  alphabet += char;
});

} 
console.log(alphabet); //prints 'abcd'
```

5. Create higher-order function called `filter` takes an array and a callback, and runs the callback on each element of the array if the return value of callback is `truthy` store in new array return the new array.

```js
// Test Your Code
function filter(arr, cb) {
 
 return arr.filter(ele => {
   return cb(ele);
  })

} 

var numbers = [1, 3, 5, 4, 7, 89, 234, 20];
let even = filter(numbers, function (n) {
  return n % 2 === 0;
});
console.log(even); // [4, 234, 20]
let odd = filter(numbers, function (n) {
  return n % 2 !== 0;
});
console.log(odd); // [1,3,5,7,89]
```