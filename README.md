## The Modern JavaScript Bootcamp
<br />

- ![100%](https://progress-bar.dev/40/?title=Done)

- [x] ![#0D64C3](https://via.placeholder.com/12/0D64C3/000000?text=+) `done`[Course Overview](#overview)
- [x] ![#0D64C3](https://via.placeholder.com/12/0D64C3/000000?text=+) `done`[Setting Up Your Computer](#setting-up)
- [x] ![#0D64C3](https://via.placeholder.com/12/0D64C3/000000?text=+) `done`[JavaScript Basics: Variables And Flow Control](#variables-and-flow-control)
- [x] ![#0D64C3](https://via.placeholder.com/12/0D64C3/000000?text=+) `done`[JavaScript Functions](#functions)
- [ ] ![#0D64C3](https://via.placeholder.com/12/0D64C3/000000?text=+) `in progress`[JavaScript Objects]
- [ ] ![#0D64C3](https://via.placeholder.com/12/0D64C3/000000?text=+) `in progress`[JavaScript Arrays]
- [ ] ![#0D64C3](https://via.placeholder.com/12/0D64C3/000000?text=+) `in progress`[JavaScripts In TheBrowser]
- [ ] ![#0D64C3](https://via.placeholder.com/12/0D64C3/000000?text=+) `in progress`[DataStorage, Libraries And More]
- [ ] ![#0D64C3](https://via.placeholder.com/12/0D64C3/000000?text=+) `in progress`[Expanding Our JavaScript Knowledge]
- [ ] ![#0D64C3](https://via.placeholder.com/12/0D64C3/000000?text=+) `in progress`[Advanced Objects And Functions]
- [ ] ![#0D64C3](https://via.placeholder.com/12/0D64C3/000000?text=+) `in progress`[Asynchronous JavaScript]
- [ ] ![#0D64C3](https://via.placeholder.com/12/0D64C3/000000?text=+) `in progress`[App Themes]
- [ ] ![#0D64C3](https://via.placeholder.com/12/0D64C3/000000?text=+) `in progress`[Cutting Edge JavaScript With Babel]
- [ ] ![#0D64C3](https://via.placeholder.com/12/0D64C3/000000?text=+) `in progress`[Wrapping UP]


## Overview

- JavaScript is a greate language to know, JavaScript used from web apps to server side code to native mobile applications.

- we're going to build incrementally on your knowledge, starting with the fundamentals and moving on to the most advanced language features along the way.

- There's also 90 challenges to give you real world problem solving experience.

- The course itself is broken into three parts.

    - In part one, we're going to start with the very fundamentals of the language will be installing some program and going to start to build the task manager and note taking applications.

    - In part two, we're going to take what we learned about JavaScript and we're going to connect it to a interface, we'll be putting the finishing touches on the task manager and note applications.

    - In part three, we're going to move on to the third and final app, our hangmen word game,we're going to explore asynchronous programming with JavaScript, and going to learn how to connect your application to third party data sources, This is going to allow us to send data off to be saved or to fetch data that we want to use in our applications, such as a new puzzle for the hangman game.

    - Being able to connect your app to third party data sources is essential for creating something real world.

## Setting Up

1. Inatalling Visual Studio Code [VScode](https://code.visualstudio.com/download)

- This is text editor that we will be using to write code.
- Install some extenstion like 
    - JavaScript (ES6) code snippets 
    - Sublime Text Keymap 

2. Installing Node.js [Nodejs](https://nodejs.org/en/download/)

- This is going to allow us to run JavaScript files on your machine.


3. Install cmder [Windows Only] [Cmder](https://cmder.net/)

- This is a console emulator for Windows.

## Variables And Flow Control

#### Rules Variable Names
1. You can't define a variable more than once
2. There are rules related to variable names
    *  Variable names cannot contain spaces.
    * Variable names must begin with a letter, an underscore _ or a dollar sign ($).
    * Variable names can only contain letters, numbers, underscores, or dollar signs.
    * Variable names are case-sensitive.
    * Variable names cannot be reserved keywords.

#### Notes 1
* === - equality operator
* !== - no equal operator
*  <  - less than operator
* &lt;  - grater than operator
* <=  - less than or equal to operator
* &lt;=  - greater than or equal to operator 
* &&  - Logical And operator - True if both sides are true.
* ||  - Logical Or operator - True if at least one side is ture.

#### Notes 2
- Lexical Scope (Static Scope)
- Global Scope - Defined outside of all code blocks
- Local Scope - Defined insde a code block
- In a scope you can access variables defined in that scope, or in any parent/ancestor scope.



- Challenge 1 : Solution
```js
// create variable to store city
let city = 'Kafr Elsheikh'
// create variable to store country
let country = 'Egypt'
// create variable to combine city and country
let location = city + ',' + country
// print location
console.log(location)

/* node strings.js */
```
- Challenge 2 : Solution
```js
// create variable to store fahrenheit value
let fahrenheit = 50
// create variable to store equation convert from fahrenheit to celsius
let celsius = (fahrenheit - 32) * 5 / 9
// create variable to store equation convert from fahrenheit to kelvin
let kelvin = (fahrenheit + 459.67) * 5 /9
// print celsius value 
console.log('celsius: ' + celsius)
// print kelvin vlaue
console.log('kelvin: '+ kelvin)

/* node numbers.js */
```

- Challenge 3 : Solution

```js

// create age set to your age 
let age = 70
// calculate is child - if they are 7 or under
let isChild = age <= 7
// calculate is senior - if they are 65 or older
let isSenior = age >= 65
// print is child value
console.log(isChild)
// print is senior value
console.log(isSenior)

/* node boolean.js */
```

- Challenge 4 : Solution

```js
// create age set you age
let age = 6
// If 7 or under print message about child pricing
if ( age <= 7) {
 console.log('You will get a child discount')
}

// If 65 or older print massage about senior discount
if (age >= 65){
 console.log('You will get a senior discount')
}

/* node boolean.js */
```

- Challenge 5 : Solution 

```js
// 
let temp = 45

// It is freezing outside!
if (temp <= 32){
 console.log('It is freezing outside')
}
// It is hot outside!
else if (temp >= 100){
 console.log('It is hot outside')
}
// Go for it. It is pretty nice.
else{
 console.log('Go for it. It is pretty nice')
}
/* node boolean-advanced.js */
```

- Challenge 6 : Solution
``` js
// create boolen variable one guest is vegan
let isGuestOneVegan = true
// create boolen variable two guest is vegan
let isGuestTwoVegan = false 
// Are both vegan? Only offer up vegan dishes.
if (isGuestOneVegan && isGuestTwoVegan) {
 console.log('Only offer up vegan dishes.')
}
// At least one Vegan? Make sure to offer up some vegan options.
else if (isGuestOneVegan || isGuestTwoVegan){
 console.log('Make sure to offer up some vegan options')
}
// Else, Offer up anything on the menue
else {
 console.log('Offer up anything on the menue')
}

/* node logical-and-or.js */
```

## Functions

#### Notes 3
* Function - input (argument), code, output (return vlaue)
* Undefined - undefined value when no value is assigned before using it.
    * undefined for variable
    * undefined for function arguments
    * undefined as function return default value
* Null - null as assined value
* arguments - Multiple arguments, Default arguments, 

- Challenge 7 : Solution

```js
// convertFahrenheitToCelsius
let convertFahrenheitToCelsius = function(fahrenheit){
    let celsius = (fahrenheit - 32) * 5 / 9
    return celsius
}
// call a couple of times (32) (68)
let tempOne = convertFahrenheitToCelsius(32)
let tempTwo = convertFahrenheitToCelsius(68)
// Print the converted values
console.log(tempOne)
console.log(tempTwo)

/* node functions-101.js */
```

- Challenge 8 : Solution 

```js
// function to get tip percent take two arguments total and tipPercent 
let getTip = function(total, tipPercent = .2){
    return total * tipPercent
}
let tip = getTip(100, .25)
console.log(tip)

/* node arguments.js */
```

- Challenge 9 : Solution 
```js

// Output is A 25% tip on $40 would be $10 using templete String
// function to get tip percent take two arguments total and tipPercent 
let getTip = function(total, tipPercent = .2){
    let percent = tipPercent * 100
    let tip = total * tipPercent
    return `A ${percent} tip on $${total} would be $${tip}`
}
let tip = getTip(100, .25)
console.log(tip)

/* node arguments.js */
```

- Challenge 10 : Solution
```js
// students score, total possible score
// 15/20 -> You get a C (75%)
// A 90-100, B 80-89, C 70-79, D 60-69, F 0-59

let gradeCalc = function(score, totalScore){
    let percent = (score / totalScore) * 100
    let letterGrade = ''
    
    if(percent >= 90){
        letterGrade = 'A'
    }else if (percent >= 80) {
        letterGrade = 'B'
    }else if (percent >= 70){
        letterGrade = 'C'
    }else if (percent >= 60){
        letterGrade = 'D'
    }else{
        letterGrade = 'F'
    }

    return `You get a ${letterGrade} (${percent}%)!` 

}

let result = gradeCalc(19,20)
console.log(result)

/* node grade-calc.js */
```