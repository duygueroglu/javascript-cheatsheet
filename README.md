# javascript-cheatsheet ![AUR last modified](https://img.shields.io/badge/last%20modified-today-success) ![](https://img.shields.io/badge/starred-3-orange)
That's a repository that i've learned basic tricks about javascript in Front-End Bootcamp. I hope it works for you, have a good time!

### Comment Lines
```javascript
//single line comment

/*
multiline
block
comments
*/
```
### Variable Declaration `var` `const` `let`
```javascript
var x1; //variable
var x2="name"; //string
var x3=[1,2,"string","name"]  //array
var x4=function(){};  //function
var isLogin=true; //boolean
//const, comes with ECMAScript 6 (ES6) 2015
const PI=3.14; //constant variable
const array1=['1','2','3'];

//let, comes with ES6(2015)
let number1;  //variable declaration
let number2=11; //initialization
let number3=22;
let result=number2*number3;
let word='javascript';

/* when you defining a variable,
* you can use camelCase or Snake_Case naming conventions.
* you can start with a character or an underscore(_).
* you can start with a $ symbol.
* you can't start with a number.
* you can't separate the name with a hyphen(-).
*/

```
### Comparison Operators
```javascript
/*  
* =   (value assignment)
* ==  (equal to)
* === (equal value and equal type)
* !=  (not equal) 
* !== (not equal value or not equal type)
* >   (greater than)
* >=  (greater than or equal to)
* <   (less than)
* <=  (less than or equal to)
*/
```

### Logical Operators
```javascript
/* 
* && (and)
* || (or)
* !  (not)
*/
```

### Outputs
```javascript
console.log(x1);
alert(x1);
window.alert(x1);
document.write(x1);
```

### Conditional (Ternary) Operator
```javascriptjavascript
// Using --> () ? if condition is true : if condition is false ;
let ter = (number===1) ? "number is equal to 1" : "number is not equal to 1" ;
console.log(ter);
```

### Increment `x++` `++x`- Decrement `x--` `--x`
```javascript
var x1=10;
// console.log(x1++);
// console.log(x1);

// var x1=10;
// console.log(x1--);
// console.log(x1);

// Postfix increment – decrement
// var x1=10;
// console.log(++x1);
// console.log(x1);

// var x1=10;
// console.log(--x1);
// console.log(x1);
```

### Casting
```javascript
// Number()  ==> this is now a number.
// var x1=Number("16");
// String()  ==> this is now a string.
// Boolean() ==> true false
// Symbol()  ==> its value is kept private and for internal use (comes with ES6,2015)

//All values will resolve to true except:
Boolean(false) //false
Boolean(0) //false
Boolean(NaN) //false
Boolean("") //false
Boolean(null) //false
Boolean(undefined) //false

```
### typeof, undefined, NaN
```javascript
//typeof (what's its type ? number ? boolean ?)
// var x1=true;
// console.log(typeof x1);
```

```javascript
//undefined
// var x1;
// console.log(x1);
```

```javascript
//NaN: Not A Number
// 32/"asd"
// var x1=prompt("please enter a number");
// var x2=x1*x1;
// console.log(x2);
```

### Base Convertion
```javascript
//toString(): convert any base 10 number into another base
var number=48;
console.log(sayi.toString(2));
console.log(sayi.toString(8))
console.log(sayi.toString(10))
console.log(sayi.toString(16))
```

### String Methods
```javascript
let word = 'Html5 Css3 Js Css3 '

console.log(word.length)  // how many characters
console.log(word.trim().length) // removes whitespace from both sides of a string

word=word.toLowerCase() // string is converted to lower case
console.log(word);
console.log(word.toLowerCase())

//native code
//string is converted to upper case
console.log(word.toUpperCase())

//charAt(0) ==> you give a number, it gives you the letter that corresponds to that number.
console.log(word.charAt(0));

// whitespace is a character.
// substring() is similar to slice(), the difference is that substring() cannot accept negative indexes.
console.log(word.substring(6))
console.log(word.substring(0,5)) //0<=x<5

// concat: joins two or more strings
console.log(word.concat("added later"));

//starts with ==> true
console.log(word.startsWith('H'))

//ends with ==> true
console.log(word.endsWith('l5 '))

console.log(word.indexOf('Css3'))
console.log(word.search('Css3'))
console.log(word.lastIndexOf('Css3'))

console.log(word.split(' '))
console.log(word.join())
console.log(word.replace())
console.log(word.slice())
console.log(word.repeat())


//escape characters
//back slash \
//special symbol
console.log("\"Javascript")
console.log('Javascript')
```

### Exception Handling
```javascript
// runtime errors are caught using the try-catch-finally block.

try-catch-finally:
try{
   //error may occur
} catch(e){
    //if error is occured, it runs
} finally{
    //whether or not the error occurs, it runs
}

// throw: used to throw a custom error. we can use try..catch with throw for create custom error messages.
var s1=5;
try{
    if(s1<4){
        throw "s1 is not less than 4";
    }
} catch(err){
    alert(err);
}
```

### Functions
```javascript
//1.Function: Without parameters
function calculate(){
     let number1,number2;
     number1= Math.round(Number(prompt("First number "))) ;
     number2= Math.round(Number(prompt("Second number ")))  ;
     console.log((number1 + number2));
     console.log((number1 - number2));
     console.log((number1 / number2));
     console.log((number1 * number2));
}
calculate();
```
```javascript
//2.Function: With parameters
function calculate2(number1,number2){  //parameters
     console.log((number1 + number2));
     console.log((number1 - number2));
     console.log((number1 / number2));
     console.log((number1 * number2));
}
calculate2(20,5); //arguments
```
```javascript
//3.Function: Return
//if you want to return a variable, you can use return.
function calculate3(number1){ //parameter
     let result = number1 * number2;
     return result;
}
```
```javascript
//4.Function: Anonymous function: without a name
function(){
     return "Javascript js";
}
```
```javascript
//5.Function: Arrow function
// ()=>{}
```
```javascript
//6.Function: Immediate function
// ()()
```
```javascript
function first() {
     console.log('this is a normal function')
}
first()
```
```javascript
// if you want to use anonymous function directly ===> function(){}
let result2 = function(){
     console.log('this is an anonymous function')
}
result2()
```
```javascript
//arrow function ===> ()=>{}
let result3 = () => {
     console..log('this is an arrow function')
}
result3()
```
```javascript
//immediate function
// ===> ()()
(function deneme() {
     console.log('this is an immediate function')
})()
```
### Loops
```javascript
//For loop
for(let i=2; i<=10; i+=2){
     let num=Number(prompt(i+". num"))
     console.log(num)
}
```
```javascript
//While Loop
let i=1;
while(i<=2){
     let num=Number(prompt(i+". num"))
     console.log(num)
     i+=1;
// }
```
```javascript
//Do-While Loop
do {
//whether the condition is met or not, it will definitely work once.
     console.log('ran '+ i + ' times')
     i++;
} while (i < 3);
```
### If - Else
```javascript
if(num===1){
     console.log("num equals 1");
}
else if(num===2){
     console.log("num equals 2");
}
else{ console.log("number is not equal to 1 or 2.")
```
```javascript
//Switch-Case
function result() {
     let num = Number(prompt('enter a number'))
     switch (num) {
     case 1:
     console.log('num is equals to 1') break
     case 2:
     console.log('num is equals to 2') break
     default:
     console.log('num is outside of 1<=x<=2') break
     }
}
result();
```

### Arrays / Array Methods
```javascript
let array1 = ['html5', 'css3', 'js'];  //faster, more readable
let array2 = new Array('html5', 'css3', 'js');
let array3 = [1, 2, 3, 'a', 'b', ' ', 'c', -1, -2, -3]
```
```javascript
//Adding
array1.push() // add an element to the end
array1.unshift() // add an element to the beginning
```
```javascript
//Removing
array1.pop() // remove 1 element from the end
array1.shift() // remove1 element from the beginning
```
```javascript
//Deleting
delete array1[0]  // delete the element at the index number that we want
splice()
```
```javascript
//Sorting
array1.sort() // sorts the elements of an array
array1.reverse() // reverses the order of the elements in an array
```
```javascript
//Join()
// Returns string value by combining all data in array, separates in default with comma
let array1 = ['js','html','css']
let word = array1.join()   // output: "js,html,css"
word = array1.join('')    //output: "jshtmlcss"
word = array1.join(' & ')  //output: "js&html&css"
```
```javascript
//Concat()
//It is useful for merge strings
let word1 = 'Front'
let word2 = ' End'

let merge = word1 + word2  //normal
console.log(merge)

let merge2 = word1.concat(word2) //concat
console.log(merge2)
```
```javascript
//Splice()
//Adding and removing in a mass 
let arrays = [1, 2, 3, 4, 5, 6, 7]
arrays.splice(2, 4)  //from 2. index, delete 4 index
let arrayd = [1, 2, 3, 4, 5, 6, 7]
arrayd.splice(3, 0, 'new', 'added') //from 3. index, delete 0 index, add "new" and "added" elements
```
```javascript
//Slice()
//Copying array
let oldArray = [1, 2, 3, 4, 5, 6, 7]
let newArray = oldArray.slice(3) //start from 3. index, copy until end of the array
```

### Date Tutorials
```javascript
//Date
let dating = new Date()

//get
console.log(dating.getHours())
console.log(dating.getFullYear())

//set
console.log(new Date('2022-1-1'))
console.log(new Date(1000000000))
```

### Objects
```javascript
//Object is a standalone entity, with properties and type, camelCase

//Literal Object(Arrow Function)
let object1=()=>{
   // let array1=[];
   let array = new Array();
   console.log(array1)
   // let object2={};
   let object2 = new Object();
   console.log(object2);
} object1();

//Object Function
let object2 = () => {
   let person = {
   name: 'Duygu',
   surname: 'Eroğlu'
   calc: function(value1,value2){
   return value1+value2;
   }
}
console.log(person.calc(10,10))
}
object2()

//Nested Object
let object3 = () => {
   let person = {
   name: 'Duygu',
   surname: 'Eroğlu'
   calc: function(value1,value2){
   return value1+value2;
   },
   job:{
      jobName:"Software Engineer",
      jobType:"Engineer"
   }
}
console.log(person.calc(10,10))
console.log(person.job.jobName);
}
object3()

//Object Arrays
let objectArray = () => {
   let person = {
   name: 'Duygu',
   surname: 'Eroğlu'
   calc: function(value1,value2){
   return value1+value2;
   },
   job:{
      jobName:"Software Engineer",
      jobType:"Engineer"
   },
   languages:['JS','Java','C#','Python'],
   languageProperties:{
      roles: 'xyz',
   },
}
console.log(person)
console.log(person.languages[2])
console.log(person.job.jobName);
}
objectArray()
```

- Next tricks will be added.

Author
=============
👤 Duygu Eroğlu
* Github: [@duygueroglu](https://github.com/duygueroglu "@duygueroglu")
* Linkedin: <a href="https://www.linkedin.com/in/duygu-eroglu-75428796/" target="_blank"><img src="https://img.shields.io/badge/LinkedIn-%230077B5.svg?&style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
* Instagram: <a href="https://www.instagram.com/duygu.eroglu" target="_blank"><img src="https://img.shields.io/badge/Instagram-%23E4405F.svg?&style=flat-square&logo=instagram&logoColor=white" alt="Instagram"></a>
