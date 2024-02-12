# Section 15: Intermediate Javascript.
## Random Number Generation in Javascript: Building a Love Calculator.
[Math.random()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math/random) 
[Pseudorandom number generators | Computer Science | Khan Academy](https://www.youtube.com/watch?v=GtOt7EBNEwQ)
```js
var n = Math.random();// Generate random number.
n = n * 6;
n = Math.floor(n) + 1;// Round to the nearest whole number.
console.log(n);

//Love Calculator code.
function loveCalculator(firstName, secondName){
    var randomNumber = Math.random();
    var score = randomNumber * 100;
    var scoreRounded = Math.floor(score) + 1;
    return scoreRounded;
}

var firstName = prompt("What's the name of your crush?");
var secondName = prompt("What's your name?");
var computation = loveCalculator(firstName, secondName);
var output = alert(secondName + " Your love score for you and " + firstName + " is " + computation + " %");
```
## Control Statements: Using if-else Conditionals & Logic.
```js
function loveCalculator(firstName, secondName){
    var randomNumber = Math.random();
    var score = randomNumber * 100;
    var scoreRounded = Math.floor(score) + 1;
    var result = " ";

    if(score > 70){
        result = secondName + " Your love score for you and " + firstName + " is " + computation + " %. You love each other like Kanye loves Kanye";
    }else{
        result = secondName + " Your love score for you and " + firstName + " is " + computation + " %";
    }
    return result;
}

var firstName = prompt("What's the name of your crush?");
var secondName = prompt("What's your name?");
var computation = loveCalculator(firstName, secondName);
var output = alert(computation);
```
## Combining Operators.
```js
function loveCalculator(firstName, secondName){
    
    var randomNumber = Math.random();
    var score = randomNumber * 100;
    var scoreRounded = Math.floor(score) + 1;
    var result = " ";

    if(scoreRounded > 70){
        
        result = secondName + " Your love score for you and " + firstName + " is " + computation + " %. You love each other like Kanye loves Kanye";
        
    }else if(scoreRounded > 30 && scoreRounded <= 70 ){
        
        result = secondName + " Your love score for you and " + firstName + " is " + computation + " %";
        
    }else{
        
        result = secondName + " Your love score for you and " + firstName + " is " + computation + " %. You go together like oil and water.";
        
    }
    return result;
}

var firstName = prompt("What's the name of your crush?");
var secondName = prompt("What's your name?");
var computation = loveCalculator(firstName, secondName);
var output = alert(computation);

// BMI Calculator revisited.
function bmiCalculator (weight, height) {
    var w = parseInt(weight);
    var h = parseInt(height);
    var r = Math.floor(w/(h * h));
    var interpretation = " ";
    
    if(r < 18.5){
        
        interpretation = "Your BMI is " + r + ", so you are underweight."; 
        
    }else if(r > 18.5 && r <= 24.9){
        
        interpretation = "Your BMI is " + r + ", so you have a normal weight.";  
        
    }else{
        
        interpretation = "Your BMI is " + r + ", so you are overweight."; 
    }
    return interpretation;
}
```
## Leap Year Challenge.
[Leap Year Calculator](https://www.mathsisfun.com/leap-years.html)
```js
function leapYearScenario(year){

    var result = " ";
    
    if(year % 4 === 0){
        
        result = "leap year.";
        
    }

    return result;
}

function leapYearScenarioTwo(year){

    var result = " ";
    
    if(year % 400 === 0){
        
        result = "leap year.";
        
    }

    return result;
}

function leapYearScenarioThree(year){

    var result = " ";
    
    if(year % 100 !== 0){
        
        result = "Not leap year.";
        
    }

    return result;
}

function isLeap(year){


    if(year % 4 === 0){

        oddOrEven = leapYearScenario(year);
        
    }else if(year % 400 === 0){
        
        oddOrEven =leapYearScenarioTwo(year);
        
    }else{
        oddOrEven = leapYearScenarioThree(year);
    }

    return oddOrEven;
}

var year = prompt("What year would you like to check?");
var yearType = isLeap(year);
alert("The year " + year + ", is " + yearType);

```
## Useful structures.
<table>
    <tr>
        <thead>
        <thead>
    </tr>
    <tr>
        <tbody>
            <td></td>
            <td>
                <ul>
                    <li></li>
                </ul>
            </td>
        </tbody>
    </tr>
</table>

```js

```
<table>
    <thead>
    </thead>
    <tbody>
    <tr>
        <td>Pomodoro</br> 
        </td>
        <td>
          <ul>
            <li>1 - 2/12/2024</li>
            <li>2 - 2/12/2024</li>
            <li>3 - 2/12/2024</li>
            <li>4 - 2//2024</li>
          </ul>
      </td>
      </tr>
      <tr>
        <td>Pomodoro</br> 
        </td>
        <td>
          <ul>
            <li>1 - 2/10/2024</li>
            <li>2 - 2/10/2024</li>
            <li>3 - 2/10/2024</li>
            <li>4 - 2/10/2024</li>
          </ul>
      </td>
      </tr>
      <tr>
        <td>Pomodoro</br> 
        </td>
        <td>
          <ul>
            <li>1 - 2//2024</li>
            <li>2 - 2//2024</li>
            <li>3 - 2//2024</li>
            <li>4 - 2//2024</li>
          </ul>
      </td>
      </tr>
    </tbody>
</table>