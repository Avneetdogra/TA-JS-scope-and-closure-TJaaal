1. Convert the function below into different forms of function expression.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}

// Your code goes here

let percentage = function (marks,total){
  return (marks* 100)/total;
}
let percentage = (marks,total) => (marks*100)/total
2. Write Function Declaration or Function Expression next to the function.

``
function percentage(marks, total) {
  return (marks * 100) / total;
}
``
// Your answer

//Function Declaration
let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
};

//Function Expression
let percentage = function (marks, total) {
  return (marks * 100) / total;
};
let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
};
let percentage = function (marks, total) {
  return (marks * 100) / total;
};
//Function Expression
let percentage = (marks, total) => {
  return (marks * 100) / total;
};
//Function Expression
let percentage = (marks, total) => (marks * 100) / total;
//Function Expression
3. Why is a function definition an expression in JavaScript? Give one example of function expression.

let fullName = function (fisrtName,LastName){
  return ${firstName} ${LastName};
}

4. Why is a function call an expression in JavaScript?

Function expressions are invoked to avoid polluting the global scope. Instead of your program being aware of many different functions, when you keep them anonymous, they are used and forgotten immediately

5. Write VALID and INVALID next to each example below with the reason.

```js
function add(a, b) {
  return a + b;
}
`
let five = add(2, 3); // Valid
five = add; // Vaild
five = five(10, 11); // Vaild
five = function () {
  return 'Hello';
}; // Answer


6. What is the difference between function definition and function call? Explain with an example.

A function is a group of statements that together perform a task. ... A function declaration tells the compiler about a function's name, return type, and parameters. A function definition provides the actual body of the function. The C standard library provides numerous built-in functions that your program can call

7. What is the similarities between function definition and function call?

 formal parameters used in function call

8. Is the code below valid or invalid. Explain with reason.

```js
function hello() {
  console.log('Hello World!');
}

hello.user = 'Sam'; // valid or invalid
`
function hello() {
  console.log('Hello World!');
}

hello.user = 'Sam'; //  invalid
9. What is higher order function explain with an example.

Higher order functions are functions that operate on other functions, either by taking them as arguments or by returning them

10. Explain what is callback function. Why you can pass a function inside a function?

A callback function is a function passed into another function as an argument, which is then invoked inside the outer function to complete some kind of routine or action.
