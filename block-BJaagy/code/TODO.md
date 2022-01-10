1. Create a function by your choice that accepts a callback function.

```js
function addition(num, cb) {
  return cb(num);
}
function add5(n) {
  return n + 5;
}
console.log(addition(10, add5));
```

2. Create a function by you choice that returns a function reference.

```js
function filter(num, cb) {
  return num.filter(cb);
}
function even(n) {
  return n % 2 === 0;
}
function odd(n) {
  return n % 2 !== 0;
}
console.log(filter([10, 15, 64, 81, 35, 61, 22], even));
console.log(filter([10, 15, 64, 81, 35, 61, 22], odd));
```

3. Create a higher order function called `map` that takes two inputs:
   - An array of numbers/string/boolean etc
   - A 'callback' function - a function that is applied to each element of the array (inside of the function 'map')

Have `map` return a new array filled with values that are the result of the 'callback' function on each element of the input array.

```js
// Your code goes here

function map(arr, cb) {
  return arr.map(cb);
}

// Test Your Code
function multiplyByTwo(n) {
  return n * 2;
}
map([1, 2, 3, 4, 5], multiplyByTwo); //-> [2,4,6,8,10]
multiplyByTwo(1); //-> 2
multiplyByTwo(2); //-> 4
```

4. Create a higher-order function called `forEach` taht takes an array and a callback, and runs the callback on each element of the array. `forEach` does not return anything.

```js
// Your code goes here

function forEach(arr, cb) {
  arr.forEach(cb);
}
function add(char) {
  return alphabet += char;
}

// Test Your Code
let alphabet = '';
let letters = ['a', 'b', 'c', 'd'];
forEach(letters, function (char) {
  alphabet += char;
});
console.log(alphabet); //prints 'abcd'
```

5. Create higher-order function called `filter` takes an array and a callback, and runs the callback on each element of the array if the return value of callback is `truthy` store in new array return the new array.

```js
// Test Your Code

function filter(arr, cb) {
  let newArr = [];
  newArr = arr.filter(cb);
  return newArr;
}
function evenNum(n) {
  return n % 2 === 0;
}
function oddNum(n) {
  return n % 2 !== 0;
}

var numbers = [1, 3, 5, 4, 7, 89, 234, 20];
let even = filter(numbers, function (n) {
  return n % 2 === 0;
});
console.log(even); // [4,234,20]
let odd = filter(numbers, function (n) {
  return n % 2 !== 0;
});
console.log(odd); // [1,3,5,7,89]
```
