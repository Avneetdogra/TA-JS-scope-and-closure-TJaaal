For the given code below:

re-write the code in ways that system will understand
For Example:

var username = 'Arya';
let brothers = ['John', 'Ryan', 'Bran'];

console.log(username, brothers[0]);

function sayHello(name) {
  return `Hello ${name}`;
}

let message = sayHello(username);
var nextMessage = sayHello('Test');
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
console.log(username, numbers);

var username = 'Arya';
let number = 21;

function sayHello(name) {
  return `Hello ${name}`;
}

let message = sayHello(username);
var nextMessage = sayHello('Test');
// Your code goes here

var username = undefined;
let number ;
function sayHello(name) {
  return `Hello ${name}`;
}
let message;
var nextMessage = undefined;

//Execution phase
error : number is not defined
console.log(username, numbers);
let username = 'Arya';
let number = 21;

let sayHello = function (name) {
  return `Hello ${name}`;
};

let message = sayHello(username);
var nextMessage = sayHello('Test');
// Your code goes here

let username;
let number;
let sayHello;
let message;
var nextMessage = undefined;
//Execution Phase
Error: username is not defined
let username = 'Arya';
console.log(username, numbers);

let number = 21;
let message = sayHello(username);

let sayHello = function (name) {
  return `Hello ${name}`;
};

var nextMessage = sayHello('Test');
// Your code goes here

let username;
let number;
let message;
let sayHello;
var nextMessage = undefined;
//Execution Phase
let username = "Arya"
Error : number is not defined
console.log(name);
console.log(age);
var name = 'Lydia';
let age = 21;
// Your code goes here
//Declration Phase
var name = undefined;
let age;
// Excution Phase
undefined
Error : age is not defined
function sayHi(name) {
  console.log(name);
  console.log(age);
  var name = 'Lydia';
  let age = 21;
}

sayHi();
// Your code goes here

//Declaration Phase
var name = undefined;
let age;
//Excution
function sayHi(){}
undefined
Error : cannot be access before initialazation
sayHi();
function sayHi(name) {
  console.log(name);
  console.log(age);
  var name = 'Lydia';
  let age = 21;
}
// Your code goes here

var name = undefined;
let age;
//Excution
function sayHi(){}
undefined
Error : cannot be access before initialazation
sayHi();
let sayHi = function sayHi(name) {
  console.log(name);
  console.log(age);
  var name = 'Lydia';
  let age = 21;
};
// Your code goes here

//Declaration Phase
let sayHi;
var name = undefined;
let age
//Execution Phase
Error: sayHi is not defined
let num1 = 21;
console.log(sum);
var sum = num1 + num2;
let num2 = 30;
// Your code goes here

//Declaraation 
let num1;
var sum = undefined;
let num2;
//declaration phase
let num1 = 21;
undefined;
Error : num2 is not defined
var num1 = 21;

let sum2 = addAgain(num1, num2, 4, 5, 6);

let add = (a, b, c, d, e) => {
  return a + b + c + d + e;
};
function addAgian(a, b) {
  return a + b;
}
let num2 = 200;

let sum = add(num1, num2, 4, 5, 6);
// Your code goes here

//Declation phase
var num1 = undefined;
let sum2 ;
let add;
function addAgian(a, b) {
  return a + b;
}
let num2;
let sum;
//Execution phase
var num1 = 21;
let sum2 = addAgain(num1,num2,4,5,6);
function test(a) {
  let num1 = 21;
  return add(a, num1);
}

let sum = test(100);

let add = (a, b) => {
  return a + b;
};
// Your code goes here

// declaration Phase
let sum;
let add;
//Extuction Phase
function test(a){
  //Declaration Phase
  let num1;
  //Excution Phase
  let num1 =21;
  Error : add is not defined;
}
function test(a) {
  let num1 = 21;
  return add(a, num1);
}

let sum = test(100);

function add(a, b) {
  return a + b;
}
// Your code goes here

//Declaration Phase
function test(a){}
let sum;
function add(a,b){
  return a+b;
}
//Exction Phase
function test (a){
  //Declaration Phase
  let num1;
  //Extuction phase
  let num1 =21;
  undefined;
   }