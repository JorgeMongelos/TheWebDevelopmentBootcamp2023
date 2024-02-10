# Introduction to Javascript ES6
## JavaScript Alerts - Adding behavior to websites.
[Javascript Docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[idiomatic.js](https://github.com/rwaldron/idiomatic.js)

## Data Types
<table>
        <thead>
        <thead>
        <tbody>
            <tr>
                <td>Data types</td>
                <td>
                    <ul>
                        <li>string</li>
                        <li>number</li>
                        <li>boolean</li>
                    </ul>
                </td>
            </tr>
            <tr>
                <td>Methods</td>
                <td>
                    <ul>
                        <li>alert()</li>
                        <li>clear()</li>
                        <li>prompt()</li>
                    </ul>
                </td>
            </tr>
        </tbody>
</table>

## Javascript Variables
<table>
    <tr>
        <thead>
        <thead>
    </tr>
    <tr>
        <tbody>
            <td>Variables</td>
            <td>
                <ul>
                    <li>var keyword</li>
                </ul>
            </td>
        </tbody>
    </tr>
</table>

```js
var myName = prompt("What is your name?");

alert("Your name is " + myName);
```
## Coding Exercise 1: Javascript Variables Exercise.
```js
function test() {
    var a = "3";
    var b = "8";
    
/***********Do not change the code above 👆*******/
//Write your code on lines 7 - 9:
var c = a;
a = b;
b = c;
    
/***********Do not change the code below 👇*******/

    console.log("a is " + a);
    console.log("b is " + b);
}
```
## String Concatenation.
<table>
    <tr>
        <thead>
        <thead>
    </tr>
    <tr>
        <tbody>
            <td>String</br> Contactenation</td>
            <td>
                <ul>
                    <li>console.log("a is " + a);</li>
                    <li>console.log("b is " + b);</li>
                </ul>
            </td>
        </tbody>
    </tr>
</table>

```js
var message = "Hello";
var name = "Angela";

alert(message + " there, " + " " + name);
```
## String Lengths and Retrieving the Number of Characters.
```js
var tweet = prompt("Write a tweet of 182 characters or less");
var tweetCount = 182;
var remainingCharacters = characterLimit - tweet.length;

if(tweet.length <= tweetCount){
    
    console.log("You've writen " + tweet.length + " characters. You have " + remainingCharacters + " characters left.");
    
} else {

    console.log("You've reached the character limit: " + remainingCharacters);
    
}
```
## Slicing and Extracting Parts of a String.
```js
//Sample
var name = "Jorge";
name.slice(0,1); // = "J"

var name = "Jorge";
name.slice(3,4); // = "e"

var name = "Jorge";
name.slice(0,3); // = "Jor"

var name = "Jorge";
name.slice(1,4); // = "org"

//Lecture Exercise.
var tweet = prompt("Compose your tweet");
var tweetCount = 182;
var tweetUnder = tweet.slice(0,182);
var tweetModulo = tweetCount - tweet.length;

if(tweet.length < tweetCount || tweet.length == tweetCount){

   alert(" You have written " + tweet.length + ". You have " + tweetModulo +" characters left. " + tweetUnder); 
}
else{

    alert("You've surpassed the character limit: " + tweet.length + " characters. " + tweetUnder);
}
```
## Challenge: Changing String Casing.
[JS slice() method docs](https://www.w3schools.com/jsref/jsref_slice_string.asp)
```js
var name = prompt("What is your name?");
var nameCapitalized = name.slice(0,1).toUpperCase() + name.slice(1).toLowerCase();
alert("Hello " + nameCapitalized);
```
## Basic Arithmetic and the Modulo Operator in JavaScript.
```js
var dogAge = Number(prompt("What's your dog's age?"));
var humanAge = ((dogAge - 2) * 4) + 21;
alert("Your dog is: " + humanAge + " years old in human age.");
```
## Functions Part 1: Creating and Calling Functions.
[The Karel Robot Challenge](https://web.stanford.edu/~cpiech/karel/ide.html)
```js
// First Challenge.
function main(){
   goOppositeCorner();
}

function goOppositeCorner(){

   moveFourTimes()
   turnLeft();
   moveFourTimes()

}

function moveFourTimes(){

   move();
   move();
   move();
   move();

}

// Second Challenge.
function main(){
   
   putBeeper();
   diagonalMoveAndBeeper();
   diagonalMoveAndBeeper();
   diagonalMoveAndBeeper();
   diagonalMoveAndBeeper();
}

function diagonalMoveAndBeeper(){

   move();
   turnLeft();
   move();
   putBeeper();
   turnRight();
   
}

// Third Challenge(YES!)
function main(){

   initiaLine();
   oddLine();
   evenLine();
   oddLine();
   evenLine();

}

function initiaLine(){
   
   putBeeper();
   move();
   move();
   putBeeper();
   move();
   move();
   putBeeper();
   
}

function oddLine(){
   
   turnLeft();
   move();
   turnLeft();
   move();
   putBeeper();
   move();
   move();
   putBeeper();
   turnRight();
   move();
   
}

function evenLine(){
   
   turnLeft(); 
   move();
   putBeeper();
   turnRight();
   turnRight();
   move();
   move();
   putBeeper();
   move();
   move();
   putBeeper();   
   
}
```
## Functions Part 2: Parameters and Arguments.
```js
function getMilk(bottles, price){

    var cost= Math.floor(bottles * price);
    console.log("Leave house");
    console.log("Move right");
    console.log("Move right");
    console.log("Move up");
    console.log("Move up");
    console.log("Move up");
    console.log("Move up");
    console.log("Move right");
    console.log("Move right");
    console.log("Buy " + bottles + " bottles of milk at " + price);
    console.log("Calculate total cost");
    console.log("Your total cost is: " + cost + " dollars");
    console.log("Move left");
    console.log("Move left");
    console.log("Move down");
    console.log("Move down");
    console.log("Move left");
    console.log("Move left");
    console.log("Enter house");

}
```
## Coding Exercise 2: Life in Weeks Coding Exercise.
```js
function lifeInWeeks(age) {
    
/************Don't change the code above************/    
    
    //Write your code here.
    var ageAsInt = parseInt(age);
    var yearsRemaining = 90 - ageAsInt;
    var daysRemaining = yearsRemaining * 365;
    var weeksRemaining = yearsRemaining * 52;
    var monthsRemaining = yearsRemaining * 12;
    console.log("You have " + daysRemaining + " days " + weeksRemaining + " weeks and " + monthsRemaining + " months left");

/*************Don't change the code below**********/
}
lifeInWeeks(39);
```
## Coding Exercise 3: BMI Calculator.
```js
//Create your function below this line.
//The first parameter should be the weight and the second should be the height.
function bmiCalculator(weight, height){

    var w = parseInt(weight);
    var h = parseInt(height);
    var r = Math.floor(w/(h * h)); 
    return r;
    
}

var bmi = bmiCalculator(65, 1.8);
/* If my weight is 65Kg and my height is 1.8m, I should be able to call your function like this:

var bmi = bmiCalculator(65, 1.8); 

bmi should equal 20 when it's rounded to the nearest whole number.

*/
```
