1. Convert the function below into different forms of function expression.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}

// Your code goes here

let percentage = function (marks, total) {
  return (marks * 100) / total;
}

let percentage = (marks, total) => {
  return (marks * 100) / total;
}

```

2. Write Function Declaration or Function Expression next to the function.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}
// Function Declaration
```

```js
let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
};

// Function Expression
```

```js
let percentage = function (marks, total) {
  return (marks * 100) / total;
};

// Function Expression
```

```js
let percentage = (marks, total) => {
  return (marks * 100) / total;
};

// Function Expression
```

```js
let percentage = (marks, total) => (marks * 100) / total;

// Function Expression
```

3. Why is a function definition an expression in JavaScript? Give one example of function expression.


Which function are started with function key word are called function definition.
if we store the function into a variable this type  of expression are called function expression. In JavaScript.


```js
function less10 (num) {
  return num - 10;
}
// function dedeclaration

let less10 = function (num){
  return num - 10;
}

//function Expression

```
4. Why is a function call an expression in JavaScript?


As function is an object in JavaScript. Thus, if a function is stored in a variable in an expression form it's known as function expression.

5. Write VALID and INVALID next to each example below with the reason.

```js
function add(a, b) {
  return a + b;
}

let five = add(2, 3); // Valid (as the function is been called with parameters)

five = add; // Valid (as the function is not been called with parameters, it's a function reference)

five = five(10, 11); // Valid (as the function is been called with parameters, also the variable five is already reclared to store the value)

five = function () {
  return 'Hello';
}; // Valid (as it is a function expression)
```

6. What is the difference between function definition and function call? Explain with an example.

Function defination is when we define a function and function call is when we execute the function.

```js
function less10 (num) {
  return num - 10;
} // Function Defination

less10 (20); // Function call
```

7. What is the similarities between function definition and function call?

Similarty is execution of a function.

8. Is the code below valid or invalid. Explain with reason.

```js

function hello() {
  console.log('Hello World!');
}

hello.user = 'Sam'; //  valid (As function is an object in JavaScript)

```

9. What is higher order function explain with an example.

When a function defination is been passed but not a function call inside another function it is a higher order function.

```js
let number = [1, 2, 3, 4, 5, 6];
let isEven = (num) => {
  return num % 2 === 0;
}
let isOdd = (num) => {
  return num % 2 !== 0;
}
function filter (arr, cb) {
  let array = [];
  for (let i of arr) {
    if (cb(i)) {
      array.push(i);
    }
  }
  return array;
}
console.log(filter(number, isOdd));
console.log(filter(number, isEven));
```


10. Explain what is callback function. Why you can pass a function inside a function?

A function that is passed a parameter to a higher order function is known as a callback function. As function is an object in JavaScript and object is an expression, thus, a function can be passed inside a function.
