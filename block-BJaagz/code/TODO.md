Implement forEach array method using Array.reduce
forEach accepts two parameter array and callback
It does not return anything
It should work exactly like array forEach method
function forEach() {}

forEach(['Sam', 'Jon', 'Arya'], (name, i, arr) =>
  console.log(name + name, i, arr)
);
output---

function forEach(array,cb) {
Array.reduce((acc,cv,index,arr)=>{
  cb(cv,index,arr)
})
}

Array(['Sam', 'Jon', 'Arya'], (name, i, arr) =>
  console.log(name + name, i, arr)
);
Implement map array method using Array.reduce
map accepts two parameter array and callback
It returns same size of array
It should work exactly like array map method
function map(array,cb) {


 return array.reduce((acc,cv,i,arr)=>{
    acc.push(cb(cv,i,arr))
    return acc;
  },[])
  
}

map(['Sam', 'Jon', 'Arya'], (name) => name + name);
Implement filter array method using Array.reduce
filter accepts two parameter array and callback
It returns same size or smaller array
It should work exactly like array filter method
function filter() {
  // Your code goes here
}
filter(['Sam', 'Jon', 'Arya'], (name) =>
  name.startsWith('S')
); // ['Sam']

function filter(array,cb) {
  // let arr =[]
  // for(let elem of array){
  //   if (cb(elem)){
  //   arr.push(elem)
  //   }
  // }
  // return arr
//output--

return array.reduce((acc,cv,i ,arr)=>{
  if(cb(cv,i,arr)){
    acc.push(cv)
  }
  return acc
},[]);
}
filter(['Sam', 'Jon', 'Arya'], (name) =>
  name.startsWith('S')
); // ['Sam']
