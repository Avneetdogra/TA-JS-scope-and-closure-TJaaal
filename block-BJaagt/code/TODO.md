Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

Example:

function hello() {
  var username = 'Arya';
}
console.log(useranme); // username is not defind
In above code we are looking for the variable named usename. There is no variable named username in the global scope. The variable is inside the function named hello and we can't access the variable defined inside a function from outside.

The above code will throw an error Reference Error username is not defined.

Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.
{
  {
  const username = 'Arya';
}
console.log(useranme); // the above code will inside throw an error `Reference Error username is not defined`
Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.
if (true) {
  let username = 'Arya';
}
console.log(useranme); // Reference Error username is not defined
Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.
if (true) {
  let username = 'Arya';
}
console.log(useranme); // Reference Error username is not defined
Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.
let username = 'John';
if (true) {
  var username = 'Arya';
}
console.log(useranme); // 'username' has already been declared
Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.
let username = 'John';
if (true) {
  let username = 'Arya';
}
console.log(username); // john
Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.
let username = 'John';
function sayHello() {
  let username = 'Arya';
}
sayHello();
console.log(username); // john
Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.
for (var i = 0; i < 10; i++) {
  console.log(i, 'First'); // 1 to 9 is "first"
}
console.log(i, 'Second'); // 10 is second
Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.
for (let i = 0; i < 10; i++) {
  console.log(i, 'First'); // first
}
console.log(i, 'Second'); // ReferenceError: i is not defined
