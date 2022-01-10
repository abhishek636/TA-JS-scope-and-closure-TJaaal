Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

Example:

```js
function hello() {
  var username = 'Arya';
}
console.log(useranme); 

// In above code we are looking for the variable named username. There is no variable named username in the global scope. The variable is inside the function named hello and we can't access the variable defined inside a function from outside.

//The above code will throw an error Reference Error username is not defined.
```

In above code we are looking for the variable named `usename`. There is no variable named `username` in the global scope. The variable is inside the function named `hello` and we can't access the variable defined inside a function from outside.

The above code will throw an error `Reference Error username is not defined`.

2. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
{
  const username = 'Arya';
}
console.log(useranme); 

//In above code we are looking for the variable named username. There is no variable named username in the global scope. The variable is inside the { } and we can't access the variable as it's also not a function.

//The above code will throw an error Syntax Error expected expression got '{'.
```

3. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  let username = 'Arya';
}
console.log(useranme); 

//In above code we are looking for the variable named username. There is no variable named username in the global scope. The variable is inside the if condition and we can't access the variable.

//The above code will throw an error Reference Error username is not defined.
```

4. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  var username = 'Arya';
}
console.log(useranme); 

//In above code we are looking for the variable named username. There is no variable named username in the global scope. The variable inside the if condition, we can access the variable.

//The above code will give output Arya.
```

5. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  var username = 'Arya';
}
console.log(useranme); 

//In above code we are looking for the variable named username. There is a variable named username in the global scope. The variable is also redeclared inside the if condition.

//The above code will throw an error SyntaxError: redeclaration of let username.
```

6. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  let username = 'Arya';
}
console.log(useranme); 

//In above code we are looking for the variable named username. There is a variable named username in the global scope. The variable is also redeclared inside the if condition which will not be accessed, as it doesn't get inside the condition.

//The above code will give the output John.
```

7. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
function sayHello() {
  let username = 'Arya';
}
sayHello();
console.log(useranme); 

//In above code we are looking for the variable named username. There is a variable named username in the global scope. The variable is also redeclared inside the function which will be accessed, but not get assigned to the local variable.

//The above code will give the output John.
```

8. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (var i = 0; i < 10; i++) {
  console.log(i, 'First'); //  0 First 1 First 2 First 3 First 4 First 5 First 6 First 7 First 8 First 9 First 
}
console.log(i, 'Second'); //10 Second

//In above code the for loop will execute first and give the output for increment of numbers from 0 to 9 an per the condition given, then ouside the loop the incremented value of i will be displayed in the second console, as the variable i is declared through a var datatype, which is a globle scope.

```

9. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (let i = 0; i < 10; i++) {
  console.log(i, 'First'); // 0 First 1 First 2 First 3 First 4 First 5 First 6 First 7 First 8 First 9 First
}
console.log(i, 'Second'); // Reference error 'i' is not defined

//In above code the for loop will execute first and give the output for increment of numbers from 0 to 9 an per the condition given, then ouside the loop the incremented value of i will be displayed in the second console, as the variable i is declared through a let datatype, which is not a globle scope.
```
