Closure Exercise
Write a function, outer that takes an input string. Inside the function outer define another function expression named sayHello which alerts the input. sayHello should be call immediately after it is defined.
// Your code goes here
function outer(string){
  let sayHello = function (){
    alert(string)
  }
  sayHello();
}
Write a function delay that accepts two arguments, a callback and the wait for the time in milliseconds (1000 ms is 1 second). delay should return a function that, when invoked waits for the specified amount of time before executing. (Use setTimeout)
// Your code goes here
 function delay(cb,ms){
  return function(){
    setTimeout(cb,ms)
  }
}
let time = delay(()=> alert("Hello") , 2000)
time()
Write a function with a closure. The first function should only take one argument, someone's last name, and return the inner function. The returned inner function should take one more argument, someone's first name. When inner function when called it should console.log both the first name and the last name with a space.
function lastName(lastname) {
  return function firstName(firstname){
    console.log(firstname,lastname)
  }
}

let lastNameLee = lastName('lee'); // logs nothing
lastNameLee('Brett'); //logs 'Brett Lee'
This function is useful in case you want to create name for multiple people with same last name.

lastNameLee('Jane'); //logs 'Jane Lee'
lastNameLee('Lynne'); //logs 'Lynne Lee'
Create a storyWriter function that returns an object with two methods. One method, addWords adds a word to your story and returns the story while the other one, erase, resets the story back to an empty string. Here is an implementation:
function storyWriter() {
  let str = ''
  return {
    addWords: function (story) {
       str+=story
       return str
    },
    erase: function () {
      str=''
      return str
    }
  }
}

// Test
let farmLoveStory = storyWriter();
farmLoveStory.addWords('There was once a lonely cow.'); // 'There was once a lonely cow.'
farmLoveStory.addWords('It saw a friendly face.'); //'There was once a lonely cow. It saw a friendly face.'
farmLoveStory.erase(); //''

let storyOfMyLife = storyWriter();
storyOfMyLife.addWords('My code broke.'); // 'My code broke.'
storyOfMyLife.addWords('I ate some ice cream.'); //'My code broke. I ate some ice cream.'
storyOfMyLife.erase(); // ''
Create a function named forEach which accepts one parameter an array. Inside the function forEach there a variable named index which is initialized to 0.
When forEach function is called it returns another function. When the returned function is called it returns the element from the array at specific index. Every time you call the returned function the value of index should increment.

function forEach(arr) {
  let index = 0;
  return function findValue(){
    index+=1
    return arr[index-1]
  }
}

let next = forEach( [1, 2, 3, 4, 5]);
next(); // 1
next(); // 2
next(); // 3
next(); // 4
next(); // 5
Create a function named addDesignation which accepts a title and returns another function.
The returned function accepts a string prefix and returns prefix and title with a space.

function addDesignation(title) {
  return function prefix(prefix){
    return (prefix +" " +title)
  }
}

let sales = addDesignation('Salesman');
sales('Main'); // Main Salesman

let manager = addDesignation('Manager');
manager('Regional'); // Regional Manager
manager('Head'); // Head Manager
Create a function named changeSalary which accepts currentSalary (number) and returns an object that contains three methods
raise which will add 500 to the current salary and returns the updated salary
lower will decrease the salary by 500 returns the updated salary
current will return the current salary returns the updated salary
function changeSalary(slr) {
  return {
    raise(){
    return  slr + 500;
    },
    lower(){
      return slr - 500;
    },
    current(){
      return slr
    }
      

    }
  }


let sam = changeSalary(2000);
sam.raise(); // 2500

let arya = changeSalary(4000);
arya.lower(); // 3500
Create a function named nameFactory which accepts firstName and lastName and returns an object with multiple functions.
getFullName: return the full name of the person with a space
setFirstName: accepts a parameter first name using which updates the firstName and return the updated full name
setLastName: accepts a parameter last name using which updates the firstName and return the updated full name
function nameFactory(firstname, lastname){
  // let str = "";
  return {
    // getFullName:function(firstName,lastName){
    //   str  += firstname +" "+lastname
    //   return str
    // },
    
    // setFirstName:function(firstName,lastName){
    //   str  += firstname +" "+lastname
    //   return str
    // }
    getFullName(){
      return `${firstname} ${lastname}`;
    }
    setfullName(fn){
      firstName =fn;
      return `${firstname} ${lastname}`;
    }
     setLastName(ln){
lastName = fn;
return `${firstname} ${lastname}`;
     }
  }
}

let arya = nameFactory('Arya', 'Stark');
arya.getFullName(); // "Arya Stark"
arya.setFirstName('Jon'); // "Jon Stark"
arya.setLastName('Lannister'); // "Jon Lannister"
Create a function named createTag which accepts an HTML element name and returns another function.
The returned function accepts a string (children) and returns the children with the tag you passed.

function createTag(tags) {
  function str(children){
    let string = document.createElement(tags);
    string.innerText = children;
    return string;
  } 
  return str; 
}

let bold = createTag('b');
bold('Hello World!'); // <b>Hello World!</b>

let italic = createTag('i');
italic('Hello World!'); // <i>Hello World!</i>