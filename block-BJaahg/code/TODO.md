Understanding Scope and the difference between var, let and const
Watch this video before doing the exercise: https://www.youtube.com/watch?v=XgSjoHgy3Rk

Guess the output:
let firstName = 'Arya';
const lastName = 'Stark';
var knownAs = 'no one';

console.log(
  window.firstName, //undefined
  window.lastName,//undefined
  window.knownAs // 'no one'
);
Guess the output:
let firstName = 'Arya';
const lastName = 'Stark';
var knownAs = 'no one';

function fullName(a, b) {
  return a + b;
}

console.log(window.fullName(firstName, lastName));// 'Arya Stark'
Make a Execution Context Diagram for the following JS and write the output.
fucntion addOne(num){
  return num + 1;
}
var one = addOne(0);
var two = addOne(1);
console.log(one, two);
Make a Execution Context Diagram for the following JS and write the output.
var one = addOne(0);
fucntion addOne(num){
  return num + 1;
}
var two = addOne(1);
console.log(one, two);
Make a Execution Context Diagram for the following JS and write the output.
console.log(addOne(0));
fucntion addOne(num){
  return num + 1;
}
var two = addOne(1);
console.log(two);
Make a Execution Context Diagram for the following JS and write the output.
var one = addOne(0);
const addOne = (num) => {
  return num + 1;
};
var two = addOne(1);
console.log(two);
Make a Execution Context Diagram for the following JS and write the output.
console.log(addOne(0));
const addOne = (num) => {
  return num + 1;
};
var two = addOne(1);
console.log(two);
What will be the output of the following
function isAwesome() {
  var awesome;
  if (false) {
    awesome = true;
  }
  console.log(awesome);
}
isAwesome();//undefined
What will be the output of the following
function isAwesome() {
  let awesome;
  if (true) {
    awesome = true;
  }
  console.log(awesome);
}
isAwesome();//True
What will be the output of the following
function isAwesome() {
  let awesome;
  if (false) {
    awesome = true;
  }
  console.log(awesome);
}
isAwesome();//undefined
What will be the output of the following
let firstName = 'Arya';
const lastName = 'Stark';
var knownAs = 'no one';

function fullName(a, b) {
  return a + b;
}
const name = fullName(firstName, lastName);
console.log(name);//'Arya Stark'
Guess the output of the code below with a reason.
function sayHello() {
  let name = 'Arya Stark';
}
sayHello();

console.log(name);//'Arya Stark'
Guess the output of the code below with a reason.
if (true) {
  var name = 'Arya Stark';
}
console.log(name);// undefined
Guess the output of the code below with a reason.
if (true) {
  let name = 'Arya Stark';
}
console.log(name);//Arya Stark
Guess the output of the code below with a reason.
for (var i = 0; i < 20; i++) {
  
}
console.log(i); //20
Guess the output of the code below with a reason.
for (let i = 0; i < 20; i++) {
  /
console.log(i);
Guess the output and the reason behind that.
function sample() {
  if (true) {
    var username = 'John Snow';
  }
  console.log(username);
}
sample();
Guess the output and the reason behind that.
function sample() {
  if (true) {
    let username = 'John Snow';
  }
  console.log(username);
}
sample();
Guess the output and the reason behind that.
function sample() {
  var username = 'Arya Stark';
  if (true) {
    var username = 'John Snow';
    console.log(username);
  }
  console.log(username, 'second');
}
sample();
Guess the output and the reason behind that.
function sample() {
  let username = 'Arya Stark';
  if (true) {
    let username = 'John Snow';
    console.log(username, 'first');
  }
  console.log(username, 'second');
}
sample();
Guess the output and the reason behind that.
function sample(...args) {
  for (let i = 0; i < args.length; i++) {
    let message = `Hello I am ${args[i]}`;
    console.log(message);
  }
}

sample('First', 'Second', 'Third');
Guess the output and the reason behind that.
function sample(...args) {
  for (let i = 0; i < args.length; i++) {
    const message = `Hello I am ${args[i]}`;
    console.log(message);
  }
}

sample('First', 'Second', 'Third');
Guess the output and the reason behind that.
if (true) {
  const myFunc = function () {
    console.log(username, 'Second');
  };
  console.log(username, 'First');
  let username = 'Hello World!';
  myFunc();
}
Guess the output and the reason behind that.
function outer() {
  let movie = 'Mad Max: Fury Road';
  function inner() {
    console.log(
      `I love this movie called ${movie.toUpperCase()}`
    );
  }
  inner();
}

outer();
Guess the output and the reason behind that.
function outer() {
  let movie = 'Mad Max: Fury Road';
  function inner() {
    let movie = 'Before Sunrise';
    console.log(
      `I love this movie called ${movie.toUpperCase()}`
    );
  }
  inner();
}

outer();
Guess the output and the reason behind that.
function outer() {
  let movie = 'Mad Max: Fury Road';
  function inner() {
    let movie = 'Before Sunrise';
    function extraInner() {
      let movie = 'Gone Girl';
      console.log(
        `I love this movie called ${movie.toUpperCase()}`
      );
    }
    extraInner();
  }
  inner();
}
outer();
Using reduce find the final value when the initial value passed is 100. You have to pass the output of one function into the input of next function in the array allFunctions starts with addOne ends with half.
const addOne = (num) => {
  return num + 1;
};
const subTwo = (num) => {
  return num - 2;
};
const multiplyThree = (num) => {
  return num * 3;
};
const half = (num) => {
  return num / 2;
};

let allFunctions = [
  addOne,
  subTwo,
  multiplyThree,
  addOne,
  multiplyThree,
  half,
];

// Answer is: 447
