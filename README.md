# javascript-cheatsheet ![AUR last modified](https://img.shields.io/badge/last%20modified-today-success) ![](https://img.shields.io/badge/starred-2-orange)
That's a repository that i've learned basic tricks about javascript.

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
//1.Function: without parameters
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

- Next tricks will be added.

Author
=============
👤 Duygu Eroğlu
* Github: [@duygueroglu](https://github.com/duygueroglu "@duygueroglu")
* Linkedin: [Duygu Eroğlu](https://www.linkedin.com/in/duygu-eroglu-75428796/ "Duygu Eroğlu")

