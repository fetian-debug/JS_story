## The Modern JavaScript Bootcamp
|
├── 1_CourseOverview
├── 2_SettingUpYourComputer
├── 3_JavaScriptBasicsVariablesAndFlowControl
├── 4_JavaScriptFunctions
├── 5_JavaScriptObjects
├── 6_JavaScriptArrays
├── 7_JavaScriptsInTheBrowser
├── 8_DataStorage-Libraries-More
|── 9_ExpandingOurJavaScriptKnowledge
|── 10_AdvancedObjectsAndFunctions
├── 11_AsynchronousJavaScript
├── 12_AppThemes
├── 13_CuttingEdgeJavaScriptWithBabel
└── 14_WrappingUP


### Setting Up

- [Installing Visual Studio Code](https://code.visualstudio.com/download)

- [Installing Node.js](https://nodejs.org/en/)

- [Installing Cmder](https://cmder.net/)

### JavaScript Basics: Variables And FlowControl

#### Rules Variable Names
1. You can't define a variable more than once
2. There are rules related to variable names
	* Variable names cannot contain spaces.
	* Variable names must begin with a letter, an underscore _ or a dollar sign ($).
	* Variable names can only contain letters, numbers, underscores, or dollar signs.
	* Variable names are case-sensitive.
	* Variable names cannot be reserved keywords.

#### Notes 1
* === - equality operator
* !== - no equal operator
*  <  - less than operator
*  >  - grater than operator
* <=  - less than or equal to operator
* >=  - greater than or equal to operator 
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

- Challenge 7 : Solution

