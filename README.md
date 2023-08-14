# JavaScript_Learning
JS is a programming language
can be used for
- Web Developement
- Backend Development
- Desktop Applications
- Machine Learning  
Javascript code can be run through JS engines.
 JS engine is like compiler/interpreter which converts human readable form to computer understanble form(binary-0's & 1's) 
 Any latest browser can by default have JS engine.So without installing anything we can still run the JS code 
 Other than browser there are different JS engines available
- V8
- Spider Monkey
- Node JS (preferred)
## var,let,const
#### var
The var keyword creates variables which are function scoped. This means that any variable created with var is available anywhere in the function in which it is defined. 
```
function print() {
  if (true) {
    var name = "Kalyani"
  }
  console.log(name)
}
// Prints: Kalyani
```
Here name is available with print() function unlike other programming languages it will not be available after if block.
```
if (true) {
    var name = "Kalyani"
  }
  console.log(name)
```
Here name variable is available everywhere as it is not defined in function.

#### const/let
- let and const are block scoped which means that they are only available inside the block in which they are defined.
- const variables are constant and cannot change.
```
if (true) {
  let name = "Kalyani"
}
console.log(name)
// Uncaught ReferenceError: name is not defined
```
```
if (true) {
  let name = "Kalyani"
  console.log(name)
}
// Kalyani
```

<img width="493" alt="image" src="https://github.com/kalyani33/JavaScript_Learning/assets/37569003/2d210aa4-01a5-4b87-bff6-59f58e2617a9">  
<p> Recommended using **const** whenever you do not need to reassign the variable value, and only use ***let*** when you absolutely have to reassign a variable. </p>

## Arrow Function
```
const arr = ["Kalyani","Markram","Pedro","Pedro"];
const newarr = arr.map(ele => "Hello " + ele);
console.log(newarr);
const arr2 = arr.filter( ele => ele !== "Pedro");
console.log(arr2);
```
### Array methods
```
const items = [
    {name:"Bike",price:600},
    {name:"TV",price:500},
    {name:"Album",price:100},
    {name:"Laptop",price:400},
    {name:"Book",price:5}
];
const filteredItem = [items.filter(ele => ele.price > 400)];
console.log(filteredItem);

const printItems = items.map(item => console.log(item));

const findItem  = items.find(item => item.name=="Book");

items.forEach(item => console.log(item.name));
```

            
 
            
    
