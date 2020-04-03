
![JS](https://res.cloudinary.com/dgqqxlkfa/image/upload/v1566725872/javascript_for_everyone/javascript_for_everyone.png)

- [Introduction](#introduction)
- [Setup](#setup)
  - [Adding JavaScript to a web page](#adding-javascript-to-a-web-page)
    - [Inline Script](#inline-script)
    - [Internal script](#internal-script)
    - [External script](#external-script)
  - [Exercises:Setting Up your machine](#exercisessetting-up-your-machine)
- [Variables](#variables)
  - [Exercise - 1 : Variables](#exercise---1--variables)
- [Comments](#comments)
  - [Exercise: Comments](#exercise-comments)
- [Data types](#data-types)
  - [Primitive Data Types](#primitive-data-types)
  - [Non-Primitive Data Types](#non-primitive-data-types)
- [Numbers](#numbers)
  - [Declaring number data types](#declaring-number-data-types)
  - [Math Object](#math-object)
    - [Random number generator](#random-number-generator)
- [Strings](#strings)
  - [String Concatenation](#string-concatenation)
    - [Concatenating using addition operator](#concatenating-using-addition-operator)
    - [Long Literal Strings](#long-literal-strings)
    - [Escape Sequences in string](#escape-sequences-in-string)
    - [Template Literals(Template Strings)](#template-literalstemplate-strings)
  - [String Methods](#string-methods)
- [Checking Data types and Casting](#checking-data-types-and-casting)
  - [Checking data types](#checking-data-types)
  - [Changing data type(Casting)](#changing-data-typecasting)
    - [String to Int](#string-to-int)
    - [String to Float](#string-to-float)
    - [Float to Int](#float-to-int)
  - [Exercises: Data Types](#exercises-data-types)
    - [Exercise: String](#exercise-string)
  - [Booleans](#booleans)
    - [Exercise: Booleans](#exercise-booleans)
  - [Undefined](#undefined)
  - [Null](#null)
  - [Exercise - 6 : Data types](#exercise---6--data-types)
- [Operators](#operators)
  - [Arithmetic Operators](#arithmetic-operators)
  - [Exercises : Arithmetic Operators](#exercises--arithmetic-operators)
  - [Logical Operators](#logical-operators)
  - [Exercises: Logical Operators](#exercises-logical-operators)
  - [Comparison Operators](#comparison-operators)
  - [Exercise: Comparison Operators](#exercise-comparison-operators)
- [Conditionals](#conditionals)
  - [if](#if)
  - [if else](#if-else)
  - [if else if else](#if-else-if-else)
  - [switch](#switch)
  - [Ternary Operators](#ternary-operators)
  - [Exercise: Conditionals](#exercise-conditionals)
  - [Exercises:Local Storage](#exerciseslocal-storage)
- [Cookies](#cookies)
  - [Exercises:Cookies](#exercisescookies)
- [JavaScript Interview Questions](#javascript-interview-questions)
  - [JavaScript Tests](#javascript-tests)
  - [JavaScript Test 1](#javascript-test-1)
  - [JavaScript Test 2](#javascript-test-2)
  - [JavaScript Test 3](#javascript-test-3)

## Introduction

**_JavaScript for Everyone_** is a guide for both beginners and advanced JavaScript developers. Welcome to JavaScript. **_Congratulations_** for deciding to learn JavaScript, the language of the browser.

In this step by step tutorial, you will learn JavaScript, the most popular programming language in the history of mankind.
You use JavaScript **_to add interactivity to websites, to develop mobile apps, desktop applications, games_** and nowadays JavaScript can be used for **_machine learning_** and **_AI_**.
**_JavaScript (JS)_** has increased in popularity in recent years and has been the leading
programming language for four consecutive years and is the most used programming language on
Github.

## Setup

First thing first, lets install text or code editor. Install code editor, it could be [vscode](https://code.visualstudio.com/), [atom](https://atom.io/), [bracket](http://brackets.io/), [notepad++](https://notepad-plus-plus.org/) or others. I recommend vscode.
Install either [Chrome](https://www.google.com/chrome/) or [Firefox](https://www.mozilla.org/en-US/firefox/new/?v=b) if you didn't have yet.

If you want help, you may join the [telegram](https://t.me/JavaScriptforEveryone) channel.

### Adding JavaScript to a web page

JavaScript can be added to a web page in three ways:

- **_Inline script_**
- **_Internal script_**
- **_External script_**

The following sections show different ways of adding JavaScript code to your web page.

#### Inline Script

Create a folder on your desktop or in any location and create an **_index.html_** file in your folder. Then paste the following code and open it in a browser, either in [Chrome](https://www.google.com/chrome/) or [Firefox](https://www.mozilla.org/en-US/firefox/new/?v=b).

```html
<!DOCTYPE html>
  <html>
    <head>
      <title>JavaScript for Everyone</title>
    </head>
    <body>
      <button onclick="alert('Welcome to JavaScript!');">Click Me</button>
    </body>
  </html>
```

#### Internal script

Internal script can be written in the _head_ or the _body_ but it is preferred to put it on the body of the html document.

- Internal script  at the head

```html
<!DOCTYPE html>
  <html>
    <head>
      <title>JavaScript for Everyone</title>
      <script>
        console.log("Welcome to JavaScript for Everyone");
      </script>
    </head>
    <body>
  
    </body>
  </html>
```

- Internal script  at the body

```html
<!DOCTYPE html>
  <html>
    <head>
      <title>JavaScript for Everyone</title>
    </head>
    <body>
      <script>
        console.log("Welcome to JavaScript for Everyone");
      </script>
    </body>
  </html>
```

#### External script

The external script link can be on the head or body but it is preferred to put it in the body.

- External script  at the head

```html
<!DOCTYPE html>
  <html>
    <head>
      <title>JavaScript for Everyone</title>
      <script src="introduction.js"></script>
    </head>
    <body>
    </body>
    </html
```

- External script at the body

```html
<!DOCTYPE html>
  <html>
    <head>
      <title>JavaScript for Everyone</title>
    </head>
    <body>
      //it could be in the header or in the body
      // Here is the recommended place to put the script
      <script src="introduction.js"></script>
    </body>
    </html
```

### Exercises:Setting Up your machine

## Variables

Variables are _containers_ of data. Variables _store_ data in a memory location. When a variable is declared a memory location is reserved and when it is assigned to a value, the memory space will be filled. To declare a variable we use, _var_, _let_ or _const_ key words. For a variable which changes at different time we use _let_ but if the data doesn't change at all we use _const_. For example PI, country name, gravity.

- A JavaScript variable name  shouldn't begin with a number
- A JavaScript variable name does not allow special characters except dollar sign and underscore. 
- A JavaScript variable name follow a camelCase convention.
- A JavaScript variable name shouldn't have space between words. The following are valid examples of JavaScript variables.

Valid variables in JavaScript:

```js
    firstName
    lastName
    country
    city
    capitalCity
    age
    isMarried

    first_name
    last_name
    is_married
    capital_city

    num1
    num_1
    _num_1
    $num1
    year2019
    year_2019
```

Camel case(camelCase) or the first way of declaring is conventional in JavaScript. In this material, camelCase variables will be used.

Invalid variable:

```sh
  first-name
  1_num
  num_#_1
```

Declaring variables

```js
// Declaring different variables of different data types

let firstName = 'Asabeneh'; // first name of a person
let lastName = 'Yetayeh';   // last name of a person
let country = 'Finland';    // country
let city = 'Helsinki';      // capital city
let age = 100;              // age in years
let isMarried = true;
console.log(firstName, lastName, country, city, age, isMarried); // Asabeneh, Yetayeh, Finland, Helsinki, 100, True

// Declaring variables with number values

const gravity = 9.81;                    // earth gravity  in m/s2
const boilingPoint = 100;                // water boiling point, temperature in oC
const PI = 3.14;                         // geometrical constant
console.log(gravity, boilingPoint, PI);  // 9.81, 100, 3.14

// Variables can also be declaring in one line separated by comma

let name = 'Asabeneh', //name of a person
  job = 'teacher',
  live = 'Finland';
console.log(name, job, live);
```

### Exercise - 1 : Variables

1. Declare four variables without assigning values
2. Declare four variables with assigning values
3. Declare variables to store your first name, last name, marital status, country and age in multiple lines
4. Declare variables to store your first name, last name, marital status, country and age in a single line
5. Declare two variables _myAge_ and _yourAge_ and assign them initial values and log to browser console.
   Output:

   ```sh
   I am 25 years old.
   You are 30 years old.
   ```

## Comments

Commenting in JavaScript is similar to other programming languages. Comments can help to make code more readable.
There are two ways of commenting:

- _Single line commenting_
- _Multiline commenting_

```js
// let firstName = 'Asabeneh'; single line comment
// let lastName = 'Yetayeh'; single line comment
```

Multiline commenting:

```js
/*
    let location = 'Helsinki';
    let age = 100;
    let isMarried = true;
    This is a Multiple line comment
    */
```

### Exercise: Comments

1. Write a single line comment which says, _comments can make code readable_
1. Write a multiline comment which says, _comments can make code readable, easy to use_
   _and informative_

## Data types

In the previous section, we mentioned a little bit about data types. Data or values have data types. Data types describe the characteristics of data. Data types can be divided into two

1. Primitive data types
2. Non-primitive data types(Object References)

### Primitive Data Types

Primitive data types in JavaScript includes:

 1. Numbers - Integers, floats
 2. Strings - Any data under single or double quote
 3. Booleans - true or false value
 4. Null - empty value or no value
 5. Undefined - a declared variable without a value

Non-primitive data types in JavaScript includes:

1. Objects
2. Functions
3. Arrays

Now, let us see what exactly mean primitive and non-primitive data types.
*Primitive* data types are immutable(non-modifiable) data types. Once a primitive data type is created we can not modify it.
**Example:**

```js
let word = 'JavaScript'
```

If we try to modify the string stored in variable *word*, JavaScript will raise an error. Any data type under a single quote, double-quote, or backtick is a string data type.

```js
word[0] = 'Y'
```

This expression does not change the string stored in the variable *word*. So, we can say that strings are not modifiable or immutable.
Primitive data types are compared by its values. Let us compare different data values. See the example below:

```js
let numOne = 3
let numTwo = 3

console.log(numOne == numTwo)      // true

let js = 'JavaScript'
let py = 'Python'

console.log(js == py)             //false 

let lightOn = true
let lightOff = false

console.log(lightOn == lightOff) // false
```

### Non-Primitive Data Types

*Non-primitive* data types are modifiable or mutable. We can modify the value of non-primitive data types after it gets created.
Let us see by creating an array. An array is a list of data values in a square bracket. Arrays can contain the same or different data types. Array values are referenced by their index. In JavaScript array index starts at zero. I.e., the first element of an array is found at index zero, the second element at index one, and the third element at index two, etc.

```js
let nums = [1, 2, 3]
nums[0] = 10

console.log(nums)  // [10, 2, 3]
```

As you can see, an array in which a non-primitive data type is mutable. Non-primitive data types can not be compared by value. Even if two non-primitive data types have the same properties and values, they are not strictly equal.

```js
let nums = [1, 2, 3]
let numbers = [1, 2, 3]

console.log(nums == numbers)  // false

let userOne = {
name:'Asabeneh',
role:'teaching',
country:'Finland'
}

let userTwo = {
name:'Asabeneh',
role:'teaching',
country:'Finland'
}

console.log(userOne == userTwo) // false
```

Rule of thumb, we do not compare non-primitive data types. Do not compare array, function, or object.
Non-primitive values are referred to as reference types because they are being compared by reference instead of value. Two objects are only strictly equal if they refer to the same underlying object.

```js
let nums = [1, 2, 3]
let numbers = nums

console.log(nums == numbers)  // true

let userOne = {
name:'Asabeneh',
role:'teaching',
country:'Finland'
}

let userTwo = userOne

console.log(userOne == userTwo)  // true
```

If you have a hard time understanding the difference between primitive data types and non-primitive data types, you are not the only one. Calm down and just go to the next section and try to come back after some time. Now let us start the data types by number type.

## Numbers

Numbers are integers and decimal values which can do all the arithmetic operations.
Lets' see some examples of Numbers.

### Declaring number data types

```js
let age = 35
const gravity = 9.81  //we use const for non-changing values, gravitational constant in  m/s2
let mass = 72         // mass in Kilogram
const PI = 3.14       // pi a geometrical constant

//More Examples
const boilingPoint = 100 // temperature in oC, boiling point of water which is a constant
const bodyTemp = 37      // oC average human body temperature, which is a constant

console.log(age, gravity, mass, PI, boilingPoint, bodyTemp)
```

### Math Object

In JavaScript the Math Object provides a lots of methods to work with numbers.

```js
const PI = Math.PI

console.log(PI)                           // 3.141592653589793

// Rounding to the closest number
// if above .5 up if less 0.5 down rounding

console.log(Math.round(PI))               // 3 to round values to the nearest number

console.log(Math.round(9.81))             // 10

console.log(Math.floor(PI))               // 3 rounding down

console.log(Math.ceil(PI))                // 4 rounding up

console.log(Math.min(-5, 3, 20, 4,5, 10)) // -5, returns the minimum value

console.log(Math.max(-5, 3, 20, 4,5, 10)) // 20, returns the maximum value

const randNum = Math.random() // creates random number between 0 to 0.999999
console.log(randNum)

// Let us  create random number between 0 to 10

const num = Math.floor(Math.random () * 11) // creates random number between 0 and 10
console.log(num)

//Absolute value
console.log(Math.abs(-10))      //10

//Square root
console.log(Math.sqrt(100))     // 10

console.log(Math.sqrt(2))      //1.4142135623730951

// Power
console.log(Math.pow(3, 2)) // 9

console.log(Math.E) // 2.718

// Logarithm
//Returns the natural logarithm of base E of x, Math.log(x)
console.log(Math.log(2))    // 0.6931471805599453
console.log(Math.log(10))   // 2.302585092994046

// Trigonometry
Math.sin(0)
Math.sin(60)

Math.cos(0)
Math.cos(60)
```

#### Random number generator

The JavaScript Math Object has a random() method number generator which generates number from 0 to 0.999999999...

```js
let randomNum = Math.random() // generates 0 to 0.999
```

Now, let us see how we can use random() method to generate a random number between 0 and 10 inclusive.

```js
let randomNum = Math.random()         // generates 0 to 0.999
let numBtnZeroAndTen = randomNum * 11

console.log(numBtnZeroAndTen)         // this gives: min 0 and max 10.99

let randomNumRoundToFloor = Math.floor(numBtnZeroAndTen)
console.log(randomNumRoundToFloor)    // this gives between 0 and 10
```

## Strings

Strings are texts, which are under **_single_** or **_double_** quote. To declare a string, we need a variable name, assignment operator, a value under a single quote, double-quote, or backtick.
Lets' see some examples of string:

```js
let space = ' '           // an empty space string
let firstName = 'Asabeneh'
let lastName = 'Yetayeh'
let country = 'Finland'
let city = 'Helsinki'
let language = 'JavaScript'
let job = 'teacher'
```

### String Concatenation

Connect two or more strings together is called concatenation.

```js
// Declaring different variables of different data types
let space = ' '
let firstName = 'Asabeneh'
let lastName = 'Yetayeh'
let country = 'Finland'
let city = 'Helsinki'
let language = 'JavaScript'
let job = 'teacher'
```

```js
let fullName = firstName + space + lastName; // concatenation, merging two string together.
console.log(fullName);
```

```sh
Asabeneh Yetayeh
```

We can concatenate string in different ways.

#### Concatenating using addition operator

Concatenating using the addition operator is an old way. This way of concatenating is tedious and error-prone. It is good to know how to concatenate this way, but I strongly suggest to use the second way.

```js
// Declaring different variables of different data types
let space = ' '
let firstName = 'Asabeneh'
let lastName = 'Yetayeh'
let country = 'Finland'
let city = 'Helsinki'
let language = 'JavaScript'
let job = 'teacher'
let age = 250
let fullName = firstName + space + lastName

let personInfoOne = fullName + '. I am ' + age + '. I live in ' + country; // ES5

console.log(personInfoOne)
```

```sh
Asabeneh Yetayeh. I am 250. I live in Finland
```

#### Long Literal Strings

A string could be a single character or paragraph or a page. If the string length is too big it does not fit in one line. We can use the backslash character (\\) at the end of each line to indicate that the string will continue on the next line.
**Example:**

```js
const paragraph = "My name is Asabeneh Yetayeh. I live in Finland, Helsinki.\
I am a teacher and I love teaching. I teach HTML, CSS, JavaScript, React, Redux, \
Node.js, Python, Data Analysis and D3.js for anyone who is interested to learn. \
In the end of 2019, I was thinking to expand my teaching and to reach \
to global audience and I started a Python challenge from November 20 - December 19.\
It was one of the most rewarding and inspiring experience.\
Now, we are in 2020. I am enjoying preparing the 30DaysOfJavaScript challenge and \
I hope you are enjoying too."
console.log(paragraph)
```

#### Escape Sequences in string

In JavaScript and other programming language \ followed by some characters is  an escape sequence. Let's see the most common escape characters:

- \n: new line
- \t: Tab means(8 spaces)
- \\\\: Back slash
- \\': Single quote (')
- \\":Double quote (")
  
```js
console.log('I hope every one is enjoying the 30 Days Of JavaScript challenge.\nDo you ?') // line break
console.log('Days\tTopics\tExercises')
console.log('Day 1\t3\t5')
console.log('Day 2\t3\t5')
console.log('Day 3\t3\t5')
console.log('Day 4\t3\t5')
console.log('This is a back slash  symbol (\\)') // To write a back slash
console.log('In every programming language it starts with \"Hello, World!\"')
console.log("In every programming language it starts with \'Hello, World!\'")
console.log('The saying \'Seeing is Believing\' is\'t correct in 2020')
```

#### Template Literals(Template Strings)

To create a template string, we use two backticks. We can inject data as expression inside a template string. To inject data, we enclose the expression with a curly bracket({}) followed by a $ sign. See the syntax below.

```js
//Syntax
`String literal text`
`String literal text ${expression}`
```

**Example: 1**

```js
console.log(`The sum of 2 and 3 is 5`)              // statically writing the data
let a = 2
let b = 3
console.log(`The sum of ${a} and ${b} is ${a + b}`) // injecting the data dynamically
```

**Example:2**

```js
let firstName = 'Asabeneh'
let lastName = 'Yetayeh'
let country = 'Finland'
let city = 'Helsinki'
let language = 'JavaScript'
let job = 'teacher'
let age = 250
let fullName = firstName + ' ' + lastName

let personInfoTwo = `I am ${fullName}. I am ${age}. I live in ${country}.` //ES6 - String interpolation method
let personInfoThree = `I am ${fullName}. I live in ${city}, ${country}. I am a ${job}. I teach ${language}.`
console.log(personInfoTwo)
console.log(personInfoThree)
```

```sh
I am Asabeneh Yetayeh. I am 250. I live in Finland.
I am Asabeneh Yetayeh. I live in Helsinki, Finland. I am a teacher. I teach JavaScript.
```

Using a string template or string interpolation method, we can add expression, which could be a value or some operations(comparison, arithmetic operations, ternary operation).

```js
let a = 2
let b = 3
console.log(`${a} is greater than ${b}: ${a > b}`)
```

```sh
2 is greater than 3: false
```

### String Methods

Everything in JavaScript is an object. A string is a primitive data type that means we can not modify once it is created. The string object has many string methods. There are different string methods that can help us to work with strings.

1. *length*: The string *length* method returns the number of characters in a string included empty space.
  **Example:**

   ```js
   let js = 'JavaScript'
   console.log(js.length)         // 10
   let firstName = 'Asabeneh'
   console.log(firstName.length)  // 8
   ```

2. *Accessing characters in a string*: We can access each character in a string using its index. In programming, counting starts from 0. The first index of the string is zero, and the last index is one minus the length of the string.

  ![Accessing sting by index](../images/string_indexes.png)
  
Let us access different characters in 'JavaScript' string.

```js
let string = 'JavaScript'
let firstLetter = string[0]

console.log(firstLetter)           // J

let secondLetter = string[1]       // a
let thirdLetter = string[2]
let lastLetter = string[9]

console.log(lastLetter)            // t

let lastIndex = string.length - 1

console.log(lastIndex)  // 9
console.log(string[lastIndex])    // t
```

1. *toUpperCase()*: this method changes the string to uppercase letters.

```js
let string = 'JavaScript'

console.log(string.toUpperCase())     // JAVASCRIPT

let firstName = 'Asabeneh'

console.log(firstName.toUpperCase())  // ASABENEH

let country = 'Finland'

console.log(country.toUpperCase())    // FINLAND
```

4. *toLowerCase()*: this method changes the string to lowercase letters.

```js
let string = 'JavasCript'

console.log(string.toLowerCase())     // javascript

let firstName = 'Asabeneh'

console.log(firstName.toLowerCase())  // asabeneh

let country = 'Finland'

console.log(country.toLowerCase())   // finland
```

5. *substr()*: It takes two arguments, the starting index and number of characters to slice.

```js
let string = 'JavaScript'
console.log(string.substr(4,6))    // Script

let country = 'Finland'
console.log(country.substr(3, 4))   // land
```

6. *substring()*: It takes two arguments, the starting index and the stopping index but it doesn't include the stopping index.

```js
let string = 'JavaScript'

console.log(string.substring(0,4))     // Java
console.log(string.substring(4,10))    // Script
console.log(string.substring(4))       // Script

let country = 'Finland'

console.log(country.substring(0, 3))   // Fin
console.log(country.substring(3, 7))   // land
console.log(country.substring(3))      // land
```

7. *split()*: The split method splits a string at a specified place.

```js
let string = '30 Days Of JavaScript'

console.log(string.split())     // ["30 Days Of JavaScript"]
console.log(string.split(' '))  // ["30", "Days", "Of", "JavaScript"]

let firstName = 'Asabeneh'

console.log(firstName.split())    // ["Asabeneh"]
console.log(firstName.split(''))  // ["A", "s", "a", "b", "e", "n", "e", "h"]

let countries = 'Finland, Sweden, Norway, Denmark, and Iceland'

console.log(countries.split(','))  // ["Finland", " Sweden", " Norway", " Denmark", " and Iceland"]
console.log(countries.split(', ')) //  ["Finland", "Sweden", "Norway", "Denmark", "and Iceland"]
```

8. *trim()*: Removes trailing space in the beginning or the end of a string.

```js
let string = '   30 Days Of JavaScript   '

console.log(string)     
console.log(string.trim(' '))

let firstName = ' Asabeneh '

console.log(firstName)
console.log(firstName.trim())
```

```sh
   30 Days Of JavasCript   
30 Days Of JavasCript
  Asabeneh 
Asabeneh
```

9. *includes()*: It takes a substring argument and it check if substring argument exists in the string. *includes()* returns a boolean. It checks if a substring exist in a string and it returns true if it exists and false if it doesn't exist.

```js
let string = '30 Days Of JavaScript'

console.log(string.includes('Days'))     // true
console.log(string.includes('days'))     // false
console.log(string.includes('Script'))   // true
console.log(string.includes('script'))   // false
console.log(string.includes('java'))     // false
console.log(string.includes('Java'))     // true

let country = 'Finland'

console.log(country.includes('fin'))     // false
console.log(country.includes('Fin'))     // true
console.log(country.includes('land'))    // true
console.log(country.includes('Land'))    // false
```

10. *replace()*: takes to parameter the old substring and new substring.

```js
string.replace(oldsubstring, newsubstring)
```

```js
let string = '30 Days Of JavaScript'
console.log(string.replace('JavaScript', 'Python')) // 30 Days Of Python

let country = 'Finland'
console.log(country.replace('Fin', 'Noman'))       // Nomanland
```

11. *charAt()*: Takes index and it returns the value at that index

```js
string.charAt(index)
```

```js
let string = '30 Days Of JavaScript'
console.log(string.charAt(0))        // 3

let lastIndex = string.length - 1
console.log(string.charAt(lastIndex)) // t
```

12. *charCodeAt()*: Takes index and it returns char code(ASCII number) of the value at that index

```js
string.charCodeAt(index)
```

```js
let string = '30 Days Of JavaScript'
console.log(string.charCodeAt(3))        // D ASCII number is 51

let lastIndex = string.length - 1
console.log(string.charCodeAt(lastIndex)) // t ASCII is 116

```

1.  *indexOf()*: Takes a substring and if the substring exists in a string it returns the first position of the substring if does not exist it returns -1

```js
string.indexOf(substring)
```

```js
let string = '30 Days Of JavaScript'

console.log(string.indexOf('D'))          // 3
console.log(string.indexOf('Days'))       // 3
console.log(string.indexOf('days'))       // -1
console.log(string.indexOf('a'))          // 4
console.log(string.indexOf('JavaScript')) // 11
console.log(string.indexOf('Script'))     //15
console.log(string.indexOf('script'))     // -1
```

1.  *lastIndexOf()*: Takes a substring and if the substring exists in a string it returns the last position of the substring if it does not exist it returns -1

```js
//syntax
string.lastIndexOf(substring)
```

```js
let string = 'I love JavaScript. If you do not love JavaScript what else can you love.'

console.log(string.lastIndexOf('love'))       // 67
console.log(string.lastIndexOf('you'))        // 63
console.log(string.lastIndexOf('JavaScript')) // 38
```

15. *concat()*: it takes many substrings and creates concatenation.

```js
string.concat(substring, substring, substring)
```

```js
let string = '30'
console.log(string.concat("Days", "Of", "JavaScript")) // 30DaysOfJavaScript

let country = 'Fin'
console.log(country.concat("land")) // Finland
```

16. *startsWith*: it takes a substring as an argument and it checks if the string starts with that specified substring. It returns a boolean(true or false).

```js
//syntax
string.startsWith(substring)
```

```js
let string = 'Love is the best to in this world'

console.log(string.startsWith('Love'))   // true
console.log(string.startsWith('love'))   // false
console.log(string.startsWith('world'))  // false

let country = 'Finland'

console.log(country.startsWith('Fin'))   // true
console.log(country.startsWith('fin'))   // false
console.log(country.startsWith('land'))  //  false
```

17. *endsWith*: it takes a substring as an argument and it checks if the string starts with that specified substring. It returns a boolean(true or false).

```js
string.endsWith(substring)
```

```js
let string = 'Love is the best to in this world'

console.log(string.endsWith('world'))         // true
console.log(string.endsWith('love'))          // false
console.log(string.endsWith('in this world')) // true

let country = 'Finland'

console.log(country.endsWith('land'))         // true
console.log(country.endsWith('fin'))          // false
console.log(country.endsWith('Fin'))          //  false
```

18. *search*: it takes a substring as an argument and it returns the index of the first match.

```js
string.search(substring)
```

```js
let string = 'I love JavaScript. If you do not love JavaScript what else can you love.'
console.log(string.search('love')) // 2
```

19. *match*: it takes a substring or regular expression pattern as an argument and it returns an array if there is match if not it returns null. Let us see how a regular expression pattern looks like. It starts with / sign and ends with / sign.

```js
let string = 'love'
let patternOne = /love/     // with out any flag
let patternTwo = /love/gi   // g-means to search in the whole text, i - case insensitive
```

Match syntax

```js
// syntax
string.match(substring)
```

```js
let string = 'I love JavaScript. If you do not love JavaScript what else can you love.'
console.log(string.match('love'))
```

```sh
["love", index: 2, input: "I love JavaScript. If you do not love JavaScript what else can you love.", groups: undefined]
```

```js
let pattern = /love/gi
console.log(string.match(pattern))   // ["love", "love", "love"]
```

Let us extract numbers from text using regular expression. This is not regular expression section, no panic, we will cover regular expression in other section.

```js
let txt = 'In 2019, I run 30 Days of Python. Now, in 2020 I super exited to start this challenge'
let regEx = /\d+/

// d with escape character means d not a normal d instead acts a digit
// + means one or more digit numbers,
// if there is g after that it means global, search everywhere.

console.log(txt.match(regEx))  // ["2", "0", "1", "9", "3", "0", "2", "0", "2", "0"]
console.log(txt.match(/\d+/g)) // ["2019", "30", "2020"]
```

20.   *repeat()*: it takes a number argument and it returned the repeated version of the string.

```js
string.repeat(n)
```

```js
let string = 'love'
console.log(string.repeat(10)) // lovelovelovelovelovelovelovelovelovelove
```

## Checking Data types and Casting

### Checking data types

- Check Data types: To check the data type of a certain data type we use the _typeof_ and we also change one data type to another.
  **Example:**

```js
// Different javascript data types
// Let's declare different data types

let firstName = 'Asabeneh'      // string
let lastName = 'Yetayeh'        // string
let country = 'Finland'         // string
let city = 'Helsinki'           // string
let age = 250                   // number, it is not my real age, do not worry about it
let job                         // undefined, because a value was not assigned

console.log(typeof 'Asabeneh')  // string
console.log(typeof firstName)   // string
console.log(typeof 10)          // number
console.log(typeof 3.14)        // number
console.log(typeof true)        // boolean
console.log(typeof false)       // boolean
console.log(typeof NaN)         // number
console.log(typeof job)         // undefined
console.log(typeof undefined)   // undefined
console.log(typeof null)        // object
```

### Changing data type(Casting)

- Casting: Converting one data type to another data type. We use _parseInt()_, _parseFloat()_, _Number()_, _+ sign_, _str()_
  When we do arithmetic operations string numbers should be first converted to integer or float if not it returns an error.

#### String to Int

We can convert string number to a number. Any number inside a quote is a string number.  An example of a string number: '10', '5', etc.
We can convert string to number using the following methods:

- parseInt()
- Number()
- Plus sign(+)

```js
let num = '10'
let numInt = parseInt(num)
console.log(numInt) // 10
```

```js
let num = '10'
let numInt = Number(num)

console.log(numInt) // 10
```

```js
let num = '10'
let numInt = +num

console.log(numInt) // 10
```

#### String to Float

We can convert string float number to a float number. Any  float number inside a quote is a string float number.  An example of a string float number: '9.81', '3.14', '1.44', etc.
We can convert string float to number using the following methods:

- parseFloat()
- Number()
- Plus sign(+)

```js
let num = '9.81'
let numFloat = parseFloat(num)

console.log(numFloat) // 9.81
```

```js
let num = '9.81'
let numFloat = Number(num)

console.log(numFloat) // 9.81
```

```js
let num = '9.81'
let numFloat = +num

console.log(numInt) // 9.81
```

#### Float to Int

We can convert float numbers to integers.
We use the following method to convert float to int:

- parseInt()
  
```js
let num = 9.81
let numInt = parseInt(num)

console.log(numInt) // 9
```


### Exercises: Data Types

1. Declare variables and assign string, boolean, undefined and null data types
1. The JavaScript ***typeof*** operator uses to check different data types. Check the data type of each variables from question number 1.

#### Exercise: String

1. Declare a variable name company and assign it to an initial value **'Coding Academy'**.
1. Print the string on the browser console using __console.log()__
1. Print the __length__ of the string on the browser console using _console.log()_
1. Change all the string to capital letters using __toUpperCase()__ method
1. Change all the string to lowercase letters using __toLowerCase()__ method
1. Cut(slice) out the first word of the string using __slice__, __substr()__ or __substring()__ method
1. Use __substr__ to slice out the phase __because because because__ in the following sentence:__'You cannot end a sentence with because because because is a conjunction'__
1. Check if the string contains a word __Academy__ using __includes()__ method
1. Split the __string__ into __array__ using __split()__ method
1. Split the string Coding Academy at the space using __split()__ method
1. 'Facebook, Google, Microsoft, Apple, IBM, Oracle, Amazon' __split__ the string at the comma and change it to an array.
1. Change Coding Academy to Microsoft Academy using __replace()__ method.
1. What is character at index 10 in 'Coding Academy' string use __charAt()__ method.
1. What is the character code of A in 'Coding Academy' string using __charCodeAt()__
1. Use __indexOf__ to determine the position of the first occurrence of c in Coding Academy
1. Use __lastIndexOf__ to determine the position of the last occurrence of c in Coding Academy.
1. Use __indexOf__ to find the position of the first occurrence of the word __because__ in the following sentence:__'You cannot end a sentence with because because because is a conjunction'__
1. Use __lastIndexOf__ to find the position of the first occurrence of the word __because__ in the following sentence:__'You cannot end a sentence with because because because is a conjunction'__
1. Use __search__ to find the position of the first occurrence of the word __because__ in the following sentence:__'You cannot end a sentence with because because because is a conjunction'__
1. Use __trim()__ to remove if there is trailing whitespace at the beginning and the end of a string.E.g ' Coding Academy '.
1. Use __startsWith()__ method with the string Coding Academy make the result true
1. Use __endsWith()__ method with the string Coding Academy make the result true
1. Use __match()__ method to find all the c’s in Coding Academy
1. Use __match()__ to count the number all because's in the following sentence:__'You cannot end a sentence with because because because is a conjunction'__
1. Use __concat()__ and merge 'Coding' and 'Academy' to a single string, 'Coding Academy'
1. Use __repeat()__ method to print Coding Academy 5 times
1. Calculate the total annual income of the person by extract the numbers from the following text. 'He earns 5000 euro from salary per month, 10000 euro annual bonus, 15000 euro online courses per month.'

### Booleans

Boolean value is either true or false. Any comparisons return a boolean value which is either true or false.

```js
let isLightOn = true;
let isRaining = false;
let hungry = false;
let isMarried = true;
```

#### Exercise: Booleans

Boolean value is either true or false.

1. Write three JavaScript statement which provide truthy value.
1. Write three JavaScript statement which provide falsy value.
1. Use all the following comparison operators to compare the following values: >, < >=, <=, !=, !==,===.
   Which are true or which are false ?
   1. 4 > 3
   1. 4 >= 3
   1. 4 < 3
   1. 4 <= 3
   1. 4 == 4
   1. 4 === 4
   1. 4 != 4
   1. 4 !== 4
   1. 4 != '4'
   1. 4 == '4'
   1. 4 === '4'

### Undefined

```js
let firstName;
console.log(firstName); //not defined, because it is not assigned to a value yet
```

### Null

```js
let empty = null;
console.log(empty); // -> null , means no value
```

### Exercise - 6 : Data types

String, number, boolean, null, undefined and symbol(ES6) are JavaScript primitive data types.

1. The JavaScript *typeof* operator uses to check different data types. Check the data type of each variables from question number 1.

## Operators

### Arithmetic Operators

Arithmetic operators are mathematical operators:+, -, _, /, _

```js
let numOne = 4;
let numTwo = 3;
let sum = numOne + numTwo;
let diff = numOne - numTwo;
let mult = numOne * numTwo;
let div = numOne / numTwo;
let remainder = numOne % numTwo;

console.log(sum, diff, mult, div, remainder); // ->7,1,12,1.33,1

let PI = 3.14;
let radius = 100;          // length in meter

const gravity = 9.81;      // in m/s2
let mass = 72;             // in Kilogram
const boilingPoint = 100;  // temperature in oC, boiling point of water
const bodyTemp = 37;       // body temperature in oC

// Lets calculate area of a circle

const areaOfCircle = PI * radius * radius;
console.log(areaOfCircle); // -> 314 m

// Lets calculate weight of a substance
const weight = mass * gravity;
console.log(weight); // -> 706.32 N(Newton)

// ConcatEnating string with numbers using string interpolation
/*
 The boiling point of water is 100 oC.
 Human body temperature is 37 oC.
 The gravity of earth is 9.81 m/s2.
 */
console.log(
  `The boiling point of water is ${boilingPoint} oC.\nHuman body temperature is ${body} oC.\nThe gravity of earth is ${gravity} m / s2.`
);
```

### Exercises : Arithmetic Operators

JavaScript arithmetic operators are addition(+), subtraction(-), multiplication(\*), division(/), modulus(%), increment(++) and decrement(--).

```js
let operandOne = 4;
let operandTwo = 3;
```

Using the above operands apply different JavaScript arithmetic operators

### Logical Operators

The following symbols are the common logical operators:
&&(ampersand) , ||(pipe) and !(negation).
&& gets true only if the two operands are true.
|| gets true either of the operand is true.
! negates true to false, false to true.

```js
// && ampersand example

const check = 4 > 3 && 10 > 5; // true and true -> true
const check = 4 > 3 && 10 < 5; // true and false -> false
const check = 4 < 3 && 10 < 5; // false and false -> false

// || pipe or, example

const check = 4 > 3 || 10 > 5; // true and true -> true
const check = 4 > 3 || 10 < 5; // true and false -> true
const check = 4 < 3 || 10 < 5; // false and false -> false

// ! Negation examples

let check = 4 > 3;           // -> true
let check = !(4 > 3);        // -> false
let isLightOn = true;        // -> true
let isLightOff = !isLightOn; // -> false
let isMarried = !false;      // -> true
```

### Exercises: Logical Operators

Which are true or which are false ?

1. 4 > 3 && 10 < 12
1. 4 > 3 && 10 > 12
1. 4 > 3 || 10 < 12
1. 4 > 3 || 10 > 12
1. !(4 > 3)
1. !(4 < 3)
1. !(false)
1. !(4 > 3 && 10 < 12)
1. !(4 > 3 && 10 > 12)
1. !(4 === '4')

### Comparison Operators

```js
4 > 3;
4 >= 4;
4 < 3;
4 <= 3;
4 != 3;
4 !== '4';
4 == '4';
4 === '4';
4 === 4;
```

### Exercise: Comparison Operators

Boolean value is either true or false. Any comparison return a boolean either true or false.
Use all the following comparison operators to compare the following values: >, < >=, <=, !=, !==,===.
Which are true or which are false ?

1. 4 > 3
1. 4 >= 3
1. 4 < 3
1. 4 <= 3
1. 4 == 4
1. 4 === 4
1. 4 != 4
1. 4 !== 4
1. 4 != '4'
1. 4 == '4'
1. 4 === '4'

## Conditionals

### if

We use if condition to check only on condition.

```js
if (condition) {
  // code goes here
}

let isRaining = true;
if (isRaining) {
  console.log('Remember to take your rain coat.');
}
```

### if else

When we have more than one condition we use the if and else condition.

```js
if (condition) {
  // if the condition meets, this block of code runs
} else {
  // if condition doesn't meet, this block code runs
}

let isRaining = true;
if (isRaining) {
  console.log('You need a rain coat.');
} else {
  console.log('No need for a rain coat.');
}
```

### if else if else

Whenever we have multiple conditions.

```js
// if else if else
let weather = 'sunny';
if (weather === 'rainy') {
  console.log('You need a rain coat.');
} else if (weather === 'cloudy') {
  console.log('It might be cold, you need a jacket.');
} else if (weather === 'sunny') {
  console.log('Go out freely.');
} else {
  console.log('No need for rain coat.');
}
```

### switch

Switch an alternative for if else if else

```js
var weather = 'cloudy';
switch (weather) {
  case 'rainy':
    console.log('You need a rain coat.');
    break;
  case 'cloudy':
    console.log('It might be cold, you need a jacket.');
    break;
  case 'sunny':
    console.log('Go out freely.');
    break;
  default:
    console.log(' No need for rain coat.');
    break;
}
// Switch More Examples
var dayUserInput = prompt('What day is it ?');
var day = dayUserInput.toLowerCase();
switch (day) {
  case 'monday':
    console.log('Today is Monday');
    break;
  case 'tuesday':
    console.log('Today is Tuesday');
    break;
  case 'wednesday':
    console.log('Today is Wednesday');
    break;
  case 'thursday':
    console.log('Today is Thursday');
    break;
  case 'friday':
    console.log('Today is Friday');
    break;
  case 'saturday':
    console.log('Today is Saturday');
    break;
  case 'sunday':
    console.log('Today is Sunday');
    break;

  default:
    console.log('It is not a week day.');
    break;
}
```

### Ternary Operators

Another way to write conditionals is using ternary operators.

```js
let isRaining = true;
isRaining
  ? console.log('You need a rain coat.')
  : console.log('No need for a rain coat.');
```

### Exercise: Conditionals

1. Get user input using prompt(“Enter your age:”). If user is 18 or older , give feedback:You are old enough to drive but if not 18 give feedback to wait for the years he supposed to wait for.
   Output:

   ```sh
   Enter your age: 30
   You are old enough to drive.
   ```

   Output:
  
   ```sh
   Enter your age:15
   You are left with 3 years to drive.
   ```

1. Compare the values of myAge and yourAge using if … else. Based on the comparison log to console who is older (me or you). Use prompt(“Enter your age:”) to get the age as input.
   Output:
  
   ```sh
   Enter your age: 30
   You are 5 years older than me.
   ```

1. If a is greater than b return a is greater than b else a is less than b.
   Output:

   ```sh
    let a = 4
    let b = 3
    4 is greater than 3
    ```
  
1. Write a code which give grade students according to theirs scores:
   - 80-100, A
   - 70-89, B
   - 60-69, C
   - 50-59, D
   - 0 -49, F
1. Check if the season is Autumn, Winter, Spring or Summer.
   If the user input is:
   - September, October or November, the season is Autumn.
   - December, January or February, the season is Winter.
   - March, April or May, the season is Spring
   - June, July or August, the season is Summer

## Loops

In programming languages to carry out repetitive task we use different kinds of loop. The following examples are the commonly used loops.

### For Loop

```js
// for loop structure
for(initialization, condition, increment/decrement){
  // code goes here
}
for(let i = 0; i <= 5; i++){
  console.log(i)
}

```

### While loop

```js
let i = 0;
while (i <= 5) {
  console.log(i);
  i++;
}
```

### Do while loop

```js
let i = 0;
do {
  console.log(i);
  i++;
} while (i <= 5);
```

### Exercises:Loops

1. Iterate 0 to 10 using for loop, do the same using while and do while loop.
1. Iterate 10 to 0 using for loop, do the same using while and do while loop.
1. Write a loop that makes seven calls to console.log to output the following triangle:

   ```js
       #
       ##
       ###
       ####
       #####
       ######
       #######
   ```

1. Iterate the array, ['HTML', 'CSS', 'JavaScript'] using a for loop and print out the items.
1. Use for loop to iterate from 0 to 100 and print only even numbers
1. Use for loop to iterate from 0 to 100 and print only odd numbers
1. Use for loop to iterate from 0 to 100 and print and print the sum of all numbers.

   ```js
   The sum all numbers is 5050.
   ```

1. Use for loop to iterate from 0 to 100 and print the sum of all evens and the sum of all odds.

   ```js
   The sum of all evens is 2550. And the sum of all odds is 2500.
   ```

## Arrays

In contrast to variables array can store _multiple values_. Each value in an array has an _index_ and each index has _a reference in a memory address_. Each value can be accessed by using their _indexes_. The index of an array starts from _zero_ and the last element is less by one from the length of the array.

```js
const numbers = [0, 3.14, 9.81, 37, 98.6, 100]; // set of numbers

console.log(numbers.length) // => to know the size of the array, which is 6
console.log(numbers)        // -> [0, 3.14, 9.81, 37, 98.6, 100]
console.log(numbers[0])     //  -> 0
console.log(numbers[5])     //  -> 100

let lastIndex = numbers.length - 1;
console.log(numbers[lastIndex]) -> 100
const webTechs = [
  'HTML',
  'CSS',
  'JavaScript',
  'React',
  'Redux',
  'Node',
  'MongoDB'
]; // List of web technologies

console.log(webTechs)        // all the array items
console.log(webTechs.length) // => to know the size of the array, which is 7
console.log(webTechs[0])     //  -> HTML
console.log(webTechs[6])     //  -> MongoDB

let lastIndex = webTechs.length - 1;
console.log(webTechs[lastIndex]) -> MongoDB
const countries = [
  'Albania',
  'Bolivia',
  'Canada',
  'Denmark',
  'Ethiopia',
  'Finland',
  'Germany',
  'Hungary',
  'Ireland',
  'Japan',
  'Kenya'
]; // List of countries;

console.log(countries)     // -> all countries in array
console.log(countries[0])  //  -> Albania
console.log(countries[10]) //  -> Kenya

let lastIndex = countries.length - 1;
console.log(countries[lastIndex]) -> // Kenya

const shoppingCart = [
  'Milk',
  'Mango',
  'Tomato',
  'Potato',
  'Avocado',
  'Meat',
  'Eggs',
  'Sugar'
]; // List of food products

console.log(shoppingCart)     // -> all shoppingCart in array
console.log(shoppingCart[0])  //  -> Milk
console.log(shoppingCart[7])  //  -> Sugar

let lastIndex = shoppingCart.length - 1;
console.log(shoppingCart[lastIndex]) -> // Sugar
```

### Exercise : Arrays

1. Declare an _empty_ array;
1. Declare an array with more than 5 number of items
1. Find the length of your array
1. Get the first item, the middle item and the last item of the array
1. Declare an array called _mixedDataTypes_,put different data types and in your array and the array size should be greater than 5
1. Declare an array variable name itCompanies and assign initial values Facebook, Google, Microsoft, Apple, IBM, Oracle and Amazon.
1. Print the array using _console.log()_
1. Print the number of companies in the array
1. Print the first company, middle and last company
1. Print out each company
1. Change companies to uppercase and print them out
1. Print the array like as a sentence: Facebook, Google, Microsoft, Apple, IBM,Oracle and Amazon are big IT companies.
1. Check if a certain company exists in the itCompanies array. If it exist return the company else return a company is _not found_.
1. Filter out companies which have more than one 'o' without the filter method
1. Sort the array using _sort()_ method
1. Reverse the array without _reverse_ method
1. Reverse the array using _reverse()_ method
1. Slice out the first 3 companies from the array
1. Slice out the last 3 companies from the array
1. Slice out the middle IT company or companies from the array
1. Remove the first IT company from the array
1. Remove the middle IT company or companies from the array
1. Remove the last IT company from the array
1. Remove all IT companies

## More on Arrays

There are different methods to manipulate an array. These are some of the available methods to deal with arrays:_Array,length, concat, indexOf, slice, splice, join, toString, includes, lastIndexOf, isArray, fill, push, pop, shift, unshift_
Array:To create an array.

```js
const arr = Array(); // creates an an empty array
console.log(arr);

const eightEmptyValues = Array(8); // it creates eight empty values
console.log(eightEmptyValues);     // [empty x 8]
```

- *fill*: Fill all the array elements with a static value

```js
const arr = Array();                     // creates an an empty array
console.log(arr);
const eightXvalues = Array(8).fill('X'); // it creates eight element values
console.log(eightXvalues);               // ['X', 'X','X','X','X','X','X','X']
```

- *concat*: To concatenate two arrays.

```js
const firstList = [1, 2, 3];
const secondList = [4, 5, 6];
const thirdList = firstList.concat(secondList);

console.log(thirdList); // [1,2,3,4,5,6]
```

- *length*: To know the size of the array

```js
const numbers = [1, 2, 3, 4, 5];
console.log(numbers.length); // -> 5
```

- *indexOf*: To check if an item exist in an array. If it exist it returns the index else it returns -1.

```js
const numbers = [1, 2, 3, 4, 5];

console.log(numbers.indexOf(5));  // -> 4
console.log(numbers.indexOf(0));  // -> -1
console.log(numbers.indexOf(1));  // -> 0
console.log(numbers.indexOf(6));  // -> -1
```

- *lastIndexOf* :Give the position of the last item in the array. If it exist it returns the index else it returns -1.

```js
const numbers = [1, 2, 3, 4, 5, 3, 1, 2];

console.log(numbers.lastIndexOf(2));  // -> 7
console.log(numbers.lastIndexOf(0));  // -> -1
console.log(numbers.lastIndexOf(1));  // -> 6
console.log(numbers.lastIndexOf(4));  // -> 3
console.log(numbers.lastIndexOf(6));  // -> -1
```

*includes*: To check if an item exist in an array. If it exist it returns the true else it returns false.

```js
const numbers = [1, 2, 3, 4, 5];

console.log(numbers.includes(5)); // -> true
console.log(numbers.includes(0)); // -> false
console.log(numbers.includes(1)); // -> true
console.log(numbers.includes(6)); // -> false
```

- *isArray*:  To check if the data type is an array

```js
const numbers = [1, 2, 3, 4, 5];
console.log(Array.isArray(numbers)); // -> true

const number = 100;
console.log(Array.isArray(number)); // -> false
```

- *toString*: Converts array to string

```js
const numbers = [1, 2, 3, 4, 5];
console.log(numbers.toString()); // 1,2,3,4,5

const names = ['Asabeneh', 'Mathias', 'Elias', 'Brook'];
console.log(names.toString()); // Asabeneh,Mathias,Elias,Brook
```

join:To join the elements of the array, the argument passed in the join method will be joined in the array and return as a string.

```js
const numbers = [1, 2, 3, 4, 5];
console.log(numbers.join());        // 1,2,3,4,5
const names = ['Asabeneh', 'Mathias', 'Elias', 'Brook'];
console.log(names.join());          // Asabeneh,Mathias,Elias,Brook
console.log(names.join(''));        //AsabenehMathiasEliasBrook
console.log(names.join(' '));       //Asabeneh Mathias Elias Brook
console.log(names.join(', '));      //Asabeneh, Mathias, Elias, Brook
console.log(names.join(' # '));     //Asabeneh # Mathias # Elias # Brook
```

Slice: To cut out a multiple items in range. It takes two parameters:starting and ending position. It doesn't include the ending position

```js
  const numbers = [1,2,3,4,5];
  console.log(numbers.slice()        // -> it copies all  item
  console.log(numbers.slice(0)       // -> it copies all  item
  console.log(numbers.indexOf(0, numbers.length)) // it copies all  item
  console.log(numbers.slice(1,4))    // -> [2,3,4] // it doesn't include the ending position
```

Splice: It takes three parameters:Starting position, number of times to be removed and number items to be added.

```js
  const numbers = [1, 2, 3, 4, 5];
  console.log(numbers.splice()      // -> remove all items
  console.log(numbers.splice(0,1))  // remove the first item
  console.log(numbers.splice(3, 3, 6, 7, 8)) // -> [1,2,6,7,8] //it removes two item and replace three items

```

- *push*: adding item in the end

```js
const numbers = [1, 2, 3, 4, 5];
numbers.push(6);

console.log(numbers);  // -> [1,2,3,4,5,6]

numbers.pop();         // -> remove one item from the end
console.log(numbers);  // -> [1,2,3,4,5]
```

- *pop*: Removing item in the end

```js
const numbers = [1, 2, 3, 4, 5];
numbers.pop(); // -> remove one item from the end

console.log(numbers); // -> [1,2,3,4]
```

- *shift*: Removing item in the beginning

```js
const numbers = [1, 2, 3, 4, 5];
numbers.shift(); // -> remove one item from the beginning

console.log(numbers); // -> [2,3,4,5]
```

- *unshift*: Adding item in the beginning

```js
const numbers = [1, 2, 3, 4, 5];
numbers.unshift(0);             // -> remove one item from the beginning
console.log(numbers);           // -> [0,1,2,3,4,5]
```

---

### Exercise -10 : Array Methods

```js
const shoppingCart = ['Milk','Coffee','Tea', 'Honey'];
const todoList = [
  {
    task:'Learn JavaScript',
    time:'4/3/2019 8:30',
    completed:true
  },
  {
    task:'Help some in need',
    time:'4/3/2019 4:00',
    completed:false
  },
  {
    task:'Do some physical exercises',
    time:'4/3/2019 6:00',
    completed:false
  }
]
```

## Functions

A function is a block of code designed to perform a certain task.
A function is declared by a function key word followed by a name, followed by parentheses (). A parentheses can take a parameter. If a function take a parameter it will be called with argument. A function can also take a default parameter.
A function can be declared or created in couple of ways:

- _Declaration function_
- _Expression function_
- _Anonymous function_
- _Arrow function_

### Function Declaration

```js
//function without parameter

function functionName(){
// code goes here
}
functionName() // calling function by its name and with parentheses

//function without parameter

function addTwoNumbers() {
  var numOne = 10;
  var numTwo = 20;
  var sum = numOne + numTwo;
  console.log(sum);
}
addTwoNumbers(); // function has to be called to be executed by it name

// function with one parameter

function functionName(parm1){
  //code goes her
}
functionName(parm1); // during calling or invoking one argument needed

function areaOfCircle(r){
  let area = Math.PI * r * r;
  return area;
}
console.log(areaOfCircle(10)) // should be called with one argument

function square(number) {
  return number * number;
}
console.log(square(10));

// function with two parameters
function functionName(parm1, parm2){
  //code goes her
}
functionName(parm1,parm2); // during calling or invoking two arguments needed

// Function without parameter doesn't take input, so lets make a parameter with parameter
function sumTwoNumbers(numOne, numTwo) {
  var sum = numOne + numTwo;
  console.log(sum);
}
sumTwoNumbers(10, 20); // calling functions

// If a function doesn't return it doesn't store data, so it should return
function sumTwoNumbersAndReturn(numOne, numTwo) {
  var sum = numOne + numTwo;
  return sum;
}
console.log(sumTwoNumbersAndReturn(10, 20));

function printFullName(firstName, lastName) {
  return `${firstName} ${lastName}`;
}
console.log(printFullName('Asabeneh', 'Yetayeh'));
console.log(printFullName('Dean', 'Phan'));

// function with multiple parameters
function functionName(parm1, parm2, parm3,...){
  //code goes ther
}
functionName(parm1,parm2,parm3,...) // during calling or invoking three arguments needed


// this function takes array as a parameter and sum up the numbers in the array
function sumArrayValues(arr) {
  var sum = 0;
  for (var i = 0; i < arr.length; i++) {
    sum = sum + numbers[i];
  }
  return sum;
}
const numbers = [1, 2, 3, 4, 5];
console.log(sumArrayValues(numbers));
  

const areaOfCircle = (radius) => {
      let area = Math.PI * radius * radius;
      return area;
    }
console.log(areaOfCircle(10))
```

### Function Expression

```js
//Declaration function
function square(n) {
  return n * n;
}
console.log(square(2)); // -> 4
// Function expression
const square = function(n) {
  return n * n;
};
console.log(square(2)); // -> 4
```

### Anonymous Function

```js
// Self invoking functions
(function(n) {
  return n * n;
})(2);

const x = (function(n) {
  return n * n;
})(2);
console.log(x) // 4

```

### Arrow Function

```js
const square = n => {
  return n * n;
};
console.log(square(2)); // -> 4

// if we have only one line, it can be written as follows
// Explicit return
const square = n => n * n; // -> 4
```

### Arrow Function vs Declaration Function

Arrow function and regular functions are not exactly the same.

```js

```

### Exercise - 10 : Functions

1. Declare a function _fullName_ and it print out your full name.
1. Declare a function _fullName_ and now it takes firstName, lastName as a parameter and it returns your full - name.
1. Declare a function _addNumbers_ and it takes two two parameters and it returns sum.
1. An area of a rectangle is calculated as follows: _area = length x width_. Write a function which calculates _areaOfRectangle_.
1. A perimeter of a rectangle is calculated as follows: _perimeter= 2x(length + width)_. Write a function which calculates _perimeterOfRectangle_.
1. A volume of a rectangular prism is calculated as follows: _volume = length x width x height_. Write a function which calculates _volumeOfRectPrism_.
1. Area of a circle is calculated as follows: _area = π x r x r_. Write a function which calculates _areaOfCircle_
1. Circumference of a circle is calculated as follows: _circumference = 2πr_. Write a function which calculates _circumOfCircle_
1. Density of a substance is calculated as follows:_density= mass/volume_. Write a function which calculates _density_.
1. Speed is calculated by dividing the total distance covered by a moving object divided by the total amount of time taken. Write a function which calculates a speed of a moving object, _speed_.
1. Weight of a substance is calculated as follows: _weight = mass x gravity_. Write a function which calculates _weight_.
1. Temperature in oC can be converted to oF using this formula: _oF = (oC x 9/5) + 32_. Write a function which convert oC to oF _convertCelciusToFahrenheit_.
1. Body mass index(BMI) is calculated as follows: _bmi = weight in Kg / (height x height) in m2_. Write a function which calculates _bmi_. BMI is used to broadly define different weight groups in adults 20 years old or older.Check if a person is _underweight, normal, overweight_ or _obese_ based the information given below.
   - The same groups apply to both men and women.
   - _Underweight_: BMI is less than 18.5
   - _Normal weight_: BMI is 18.5 to 24.9
   - _Overweight_: BMI is 25 to 29.9
   - _Obese_: BMI is 30 or more
1. Write a function called _checkSeason_, it takes a month parameter and returns the season:Autumn, Winter, Spring or Summer.
1. Math.max returns its largest argument. Write a function findMax that takes three arguments and returns their maximum with out using Math.max method.

   ```js
   console.log(findMax(0, 10, 5));
   10;
   console.log(findMax(0, -10, -2));
   0;
   ```

1. Linear equation is calculated as follows: _ax + b = c_. Write a function which calculates value of a linear equation, _solveLinEquation_.
1. Quadratic equation is calculated as follows: _ax2 + bx + c = 0_. Write a function which calculates value or values of a quadratic equation, _solveQuadEquation_.
1. Declare a function name _printArray_. It takes array as a parameter and it prints out each value of the array.
1. Declare a function name _swapValues_. This function swaps value of x to y.

   ```js
   swapValues(3, 4); // x => 4, y=>3
   swapValues(4, 5); // x = 5, y = 4
   ```

1. Declare a function name _reverseArray_. It takes array as a parameter and it returns the reverse of the array (don't use method).

   ```js
   console.log(reverseArray([1, 2, 3, 4, 5]));
   [5, 4, 3, 2, 1];
   console.log(reverseArray(['A', 'B', 'C']));
   ['C', 'B', 'A'];
   ```

1. Declare a function name _capitalizeArray_. It takes array as a parameter and it returns the - capitalizedarray.
1. Declare a function name _addItem_. It takes an item parameter and it returns an array after adding the item
1. Declare a function name _removeItem_. It takes an index parameter and it returns an array after removing an item
1. Declare a function name _sumOfNumbers_. It takes a number parameter and it adds all the numbers in that range.
1. Declare a function name _sumOfOdds_. It takes a number parameter and it adds all the odd numbers in that - range.
1. Declare a function name _sumOfEven_. It takes a number parameter and it adds all the even numbers in that - range.
1. Declare a function name evensAndOdds . It takes a positive integer as parameter and it counts number of evens and odds in the number.

   ```sh
   evensAndOdds(100);
   The number of odds are 50.
   The number of evens are 51.
   ```

1. Write a function which takes any number of arguments and return the sum of the arguments

   ```js
   sum(1, 2, 3); // -> 6
   sum(1, 2, 3, 4); // -> 10
   ```

1. Writ a function which generates a _randomUserIp_.
1. Write a function which generates a _randomMacAddress_
1. Declare a function name _randomHexaNumberGenerator_. When this function is called it generates a random hexadecimal number. The function return the hexadecimal number.

   ```sh
   console.log(randomHexaNumberGenerator());
   '#ee33df'
   ```
  
1. Declare a function name _userIdGenerator_. When this function is called it generates seven character id. The function return the id.

   ```sh
   console.log(userIdGenerator());
   41XTDbE
   ```

1. Modify question number n . Declare a function name _userIdGeneratedByUser_. It doesn’t take any parameter but it takes two inputs using prompt(). One of the input is the number of characters and the second input is the number of ids which are supposed to be generated.

   ```sh
   userIdGeneratedByUser()
   'kcsy2
   SMFYb
   bWmeq
   ZXOYh
   2Rgxf
   '
   userIdGeneratedByUser()
   '1GCSgPLMaBAVQZ26
   YD7eFwNQKNs7qXaT
   ycArC5yrRupyG00S
   UbGxOFI7UXSWAyKN
   dIV0SSUTgAdKwStr
   '
   ```

1. Write a function name _rgbColorGenerator_ and it generates rgb colors.

   ```sh
   rgbColorGenerator()
   rgb(125,244,255)
   ```

1. Write a function ***arrayOfHexaColors*** which return any number of hexadecimal colors in an array.
1. Write a function ***arrayOfRgbColors*** which return any number of RGB colors in an array.
1. Write a function ***convertHexaToRgb*** which converts hexa color to rgb and it returns an rgb color.
1. Write a function ***convertRgbToHexa*** which converts rgb to hexa color  and it returns an hexa color.
1. Write a function ***generateColors*** which can generate any number of hexa or rgb colors.

    ```js
      generateColors('hexa', 3)
      ['#a3e12f','#03ed55','#eb3d2b']
      generateColors('hexa', 1)
      '#b334ef'

      generateColors('rgb', 3)
      ['rgb(5, 55, 175','rgb(50, 105, 100','rgb(15, 26, 80']
      generateColors('rgb', 1)
      'rgb(33,79, 176)'
    ```

1. Call your function _shuffleArray_, it takes an array as a parameter and it returns a shuffled array
1. Call your function _factorial_, it takes a whole number as a parameter and it return a factorial of the number
1. Call your function _isEmpty_, it takes a parameter and it checks if it is empty or not
1. Call your function _sum_, it takes any number of arguments and it returns the sum.
1. Write a function called _sumOfArrayItems_, it takes an array parameter and return the sum of all the items. Check if all the array items are number types. If not give return reasonable feedback.
1. Write a function called _average_, it takes an array parameter and returns the average of the items. Check if all the array items are number types. If not give return reasonable feedback.
1. Write a function called _modifyArray_ takes array as parameter and modifies the fifth item of the array and return the array. If the array length is less than five it return 'item not found'.

    ```js
    console.log(modifyArray(['Avocado', 'Tomato', 'Potato','Mango', 'Lemon','Carrot']);
    // →['Avocado', 'Tomato', 'Potato','Mango', 'LEMON', 'Carrot']
    console.log(modifyArray(['Google', 'Facebook','Apple', 'Amazon','Microsoft',  'IBM']);
    // →['Google', 'Facebook','Apple', 'Amazon','MICROSOFT',  'IBM']
    console.log(modifyArray(['Google', 'Facebook','Apple', 'Amazon']);
    // →'Not Found'
    ```

1. Write a function called *isPrime*, which checks if a number is prime number.
1. Write a functions which checks if all items are unique in the array.
1. Write a function which checks if all the items of the array are the same data type.
1. JavaScript variable name does not support special characters or symbols except $ or _. Write a function ***isValidVariable** which check if a variable is valid or invalid variable.
1. Write a function which returns array of seven random numbers in a range of 0-9. All the numbers must be unique.

   ```js
   sevenRandomNumbers()[(1, 4, 5, 7, 9, 8, 0)];
   ```

## Object

Everything can be an object and objects do have properties and properties have values.
Creating an object literal. To create an object literal, we use two curly brackets.
An empty object

```js
const person = {};
```

Now, the person object has firstName, lastName, age, location, skills and getFullName properties. The getFullName is function inside the person object and we call it method. The _this_ key word refers to the object itself.Example of object:

```js
const person = {
  firstName: 'Asabeneh',
  lastName: 'Yetayeh',
  age: 100,
  location: 'Helsinki',
  skills: [
    'HTML',
    'CSS',
    'JavaScript',
    'React',
    'Node',
    'MongoDB',
    'Python',
    'D3.js'
  ],
  getFullName: function() {
    return `${this.firstName}${this.lastName}`;
  }
};

const rectangle = {
  length: 20,
  width: 20,
  getArea: function() {
    return this.length * this.width;
  },
  getPerimeter: function() {
    return 2 * (this.length + this.width);
  }
};
```

Getting values from an object:

```js
  const person = {
    firstName:'Asabeneh',
    lastName:'Yetayeh',
    age:100,
    location:'Helsinki',
    skills:['HTML', 'CSS', 'JavaScript', 'React','Node','MongoDB', 'Python', 'D3.js']
    getFullName:function() {
      return `${this.firstName}${this.lastName}`
    }
  }
  console.log(person.firstName);
  console.log(person.lastName);
  console.log(person.getFullName());
  // value can be accessed
  console.log(person['age');
  console.log(person['location']);
```

Setting a new keys in an object

```js
  const person = {
    firstName:'Asabeneh',
    lastName:'Yetayeh',
    age:100,
    location:'Helsinki',
    skills:['HTML', 'CSS', 'JavaScript', 'React','Node','MongoDB', 'Python', 'D3.js']
    getFullName:function() {
      return `${this.firstName}${this.lastName}`
    }
  }
  person.nationality = 'Ethiopian'
  person.live = 'Finland';
  console.log(person)
```

### Object Methods:

_Object.assign_: To copy an object without modifying the original object

```js
const person = {
  name: 'Asabeneh',
  age: 200,
  country: 'Finland',
  skills: ['HTML', 'CSS', 'JS'],
  address: {
    street: 'Heitamienkatu 16',
    pobox: 2002,
    city: 'Helsinki'
  },
  getPersonInfo: function() {
    return `I am ${this.name} and I live in ${this.country}. I am ${this.age}.`;
  }
};

//Object methods: Object.assign, Object.keys, Object.values, Object.entries
//hasOwnProperty

const copyPerson = Object.assign({}, person);
console.log(copyPerson);
```

_Object.keys_: To get keys of an objet as an array

```js
const keys = Object.keys(copyPerson);
console.log(keys); //['name', 'age', 'country', 'skills', 'address', 'getPersonInfo']
const address = Object.keys(copyPerson.address);
console.log(address); //['street', 'pobox', 'city']
```

_Object.values_:To get values of an object as an array

```js
const values = Object.values(copyPerson);
console.log(values);
```

_Object.entries_:To get the keys and values in an array

```js
const entries = Object.entries(copyPerson);
console.log(entries);
```

_hasOwnProperty_: To check if a specific key or property exist in an object

```js
console.log(copyPerson.hasOwnProperty('name'));
console.log(copyPerson.hasOwnProperty('score'));
```

### Date Object

In JavaScript current time and date is created using JavaScript Date Object.
Some of the methods to extract date object values:*getFullYear(), getMonths(), getDate(), getDay(), getHours(), getMinutes*

```js
const now = new Date ();
const year = now.getFullYear(); // return year
const month = now.getMonth() + 1; // return month(0 - 11)
const date = now.getDate(); // return date (1 - 31)
const hours = now.getHours(); // return number (0 - 23)
const minutes = now.getMinutes();// return number (0 -59)
console.log(`${date}/${month}/${year} ${hours}:${minutes}`)
```

#### Exercises: Date Object

1. Use the new Date() object to get _month, date, year, hour_ and _minute_.
1. Write a function name _displayDateTime_ which display time in this format: 10/03/2019 04:08

   ```sh
   displayDateTime()
   10/03/2019 04:08
   ```

### Exercises:Objects

1. Create an empty object called dog
1. Print the the dog object on the console
1. Add name, legs, color, age and bark properties for the dog object. The bark property is a method which return *woof woof*
1. Get name, legs, color, age and bark value from the dog object
1. Set new properties the dog object: breed, getDogInfo
1. Create an object literal called _personAccount_. It has _firstName, lastName, incomes, expenses_ properties and it has _totalIncome, totalExpense, accountInfo,addIncome, addExpense_ and _accountBalance_ methods. Incomes is a set of incomes and its description and the same for expenses.
1. Count logged in users,count users having greater than equal to 50 points from the following object.

      ```js
      const users = {
        Alex: {
          email: 'alex@alex.com',
          skills: ['HTML', 'CSS', 'JavaScript'],
          age: 20,
          isLoggedIn: false,
          points: 30
        },
        Asab: {
          email: 'asab@asab.com',
          skills: ['HTML', 'CSS', 'JavaScript', 'React', 'Redux', 'Node.js'],
          age: 25,
          isLoggedIn: false,
          points: 50
        },
        Brook: {
          email: 'daniel@daniel.com',
          skills: ['HTML', 'CSS', 'JavaScript', 'React', 'Redux'],
          age: 30,
          isLoggedIn: true,
          points: 50
        },
        Daniel: {
          email: 'daniel@alex.com',
          skills: ['HTML', 'CSS', 'JavaScript', 'Python'],
          age: 20,
          isLoggedIn: false,
          points: 40
        },
        John: {
          email: 'john@john.com',
          skills: ['HTML', 'CSS', 'JavaScript', 'React', 'Redux', 'Node.js'],
          age: 20,
          isLoggedIn: true,
          point: 50
        },
        Thomas: {
          email: 'thomas@thomas.com',
          skills: ['HTML', 'CSS', 'JavaScript', 'React'],
          age: 20,
          isLoggedIn: false,
          points: 40
        }
      };
    ```

1. Set your name in the users object without modifying the original users object
1. Get all keys or properties of users object
1. Get all the values of users object
1. ** Develop a small JavaScript library.

## Functional Programming

- *forEach*: Iterate an array elements and use for array. It takes a callback function with elements and index parameter.

```js
arr.forEach(function(element, index){
  console.log(index, element)
})
// The above code can be written using arrow function
arr.forEach((element, index) => {
  console.log(index, element)
})
// The above code can be written using arrow function and explicit return
arr.forEach((element, index) => console.log(index, element));
```

- *map*: Iterate an array elements and modify the array elements. It takes a callback function with elements and index parameter and return the modified array.

```js
const modifiedArray = arr.map(function(element,index){
  return element
});
/*Arrow function and explicit return
const modifiedArray = arr.map((element,index) => element);
*/
//Example
const numbers = [1,2,3,4,5];
const numbersSquare = numbers.map((num) => num * num) 
console.log(numbersSquare) // [1,4,9,16,25]
const names = ['Asabeneh', 'Mathias', 'Elias', 'Brook'];
const namesToUpperCase = names.map((name) => name.toUpperCase());
console.log(namesToUpperCase) //['ASABENEH', 'MATHIAS', 'ELIAS', 'BROOK']
const countries = [
  'Albania',
  'Bolivia',
  'Canada',
  'Denmark',
  'Ethiopia',
  'Finland',
  'Germany',
  'Hungary',
  'Ireland',
  'Japan',
  'Kenya'
];
const countriesToUpperCase = countries.map(function(country){
  return country.toUpperCase();
});
console.log(countriesToUpperCase)
// ['ALBANIA', 'BOLIVIA', 'CANADA', 'DENMARK', 'ETHIOPIA', 'FINLAND', 'GERMANY', 'HUNGARY', 'IRELAND', 'JAPAN', 'KENYA']
/*
// Arrow function
const countriesToUpperCase = countries.map((country) => {
  return country.toUpperCase();
})
//Explicit return arrow function
const countriesToUpperCase = countries.map(country => country.toUpperCase());
*/
```

- *Filter*: Filter out items which full fill filtering conditions

```js

// Filter countries containing land
const countriesContainingLand = countries.filter(country => country.includes('land'));
console.log(countriesContainingLand )  //['Finland', 'Ireland']

const countriesEndByia = countries.filter(country => country.includes('ia'));
console.log(countriesEndByia) //['Albania', 'Bolivia','Ethiopia']

const countriesHaveFiveLetters = countries.filter(country => country.length === 5);
console.log(countriesHaveFiveLetters ) //  ['Japan', 'Kenya']

const scores = [{name:'Asabeneh', score:95},{name:'Mathias', score:80},{name:'Elias', score:50},{name:'Martha', score:85},{name:'John', score:100}];

const scoresGreaterEight = scores.filter((score) => score.score > 80);
console.log(scoresGreaterEight) //[{name: 'Asabeneh', score: 95}, {name: 'Martha', score: 85},{name: 'John', score: 100}]
```

- *reduce*: Reduce takes a callback function. The call back function takes accumulator and current value as a parameter and returns a single value:

```js
  const numbers = [1,2,3,4,5];
  const sum = numbers.reduce((accum, curr)=> accum + curr);

  console.log(sum); // 15
```

- *every*: Check if all the elements are similar in one aspect. It returns boolean

```js
const names = ['Asabeneh', 'Mathias', 'Elias', 'Brook'];
const bools = [true, true, true, true];
const result = bools.every((b)=> {
  return b === true;
});

console.log(result) //true

const checkType = names.every((name) => typeof name ==='string');

console.log(checkDataTypes) // true;
```

- *some*: Check if some of the elements are similar in one aspect. It returns boolean

```js
const names = ['Asabeneh', 'Mathias', 'Elias', 'Brook'];
const bools = [true, true, true, true];
const result = bools.some((b)=> {
  return b === true;
});
console.log(result) //true
const checkType = names.some((name) => typeof name ==='number');
console.log(checkDataTypes) // false
```

- *find*: Return the first element which satisfies the condition

```js
const names = ['Asabeneh', 'Mathias', 'Elias', 'Brook'];
const ages = [24, 22,25,32,35,18];
const result = names.find(name =>  name.length > 7);
console.log(result) // Asabeneh
const age = ages.find((age) => age < 20);
console.log(age) // 18
```

- *findIndex*: Return the position of the first element which satisfies the condition

```js
const names = ['Asabeneh', 'Mathias', 'Elias', 'Brook'];
const ages = [24, 22,25,32,35,18];
const result = names.findIndex(name =>  name.length > 7);
console.log(result) // 0

const age = ages.findIndex((age) => age < 20);
console.log(age) // 5
```

- *sort*: The sort methods arranges the array elements either ascending or descending order. By default, the ***sort()*** method sorts values as strings.This works well for string array items but not for numbers. If number values are sorted as strings and it give us wrong result. Sort method modify the original array.  It is recommended to copy the original document before you start sorting.

- *Sorting string values*

```js
const products = ['Milk', 'Coffee', 'Sugar', 'Honey', 'Apple', 'Carrot'];
console.log(products.sort()) // ['Apple', 'Carrot', 'Coffee', 'Honey', 'Milk', 'Sugar']
//Now the original products array  is also sorted
```

- *Sorting Numeric  values*

As you can see in the example below, 100 came first after sorted in ascending order. Sort converts items to string , since '100' and other numbers compared, 1 which the beginning of the string '100' became the smallest.  To avoid this, we use a compare call back function inside the sort method, which return a negative, zero or positive.

```js
const numbers = [9.81, 3.14, 100, 37]
// Using sort method to sort number items provide a wrong result. see below
console.log(numbers.sort()) //[100, 3.14, 37, 9.81]
numbers.sort(function(a, b) {
return a - b;
})

console.log(numbers) // [3.14, 9.81, 37, 100]
numbers.sort(function(a, b) {
return b - a;
});
console.log(numbers) //[100, 37, 9.81, 3.14]

```

- *Sorting Object Arrays*

When ever we sort objects in an array. We use the object key to compare. Lets see the example below.

```js
objArr.sort(function(a, b) {
  if (a.key < b.key) return -1;
  if (a.key > b.key) return 1;
  return 0;
});

// or

objArr.sort(function(a, b) {
  if (a['key'] < b['key']) return -1;
  if (a['key'] > b['key']) return 1;
  return 0;
});

const users = [{name:'Asabeneh', age:150}, {name:'Brook', age:50}, {name:'Eyo', age:100},{name:'Elias', age:22}];
users.sort((a, b) => {
  if (a.age < b.age) return -1;
  if (a.age > b.age) return 1;
  return 0;
});

console.log(users); // sorted ascending
//[{…}, {…}, {…}, {…}]
```

### Exercises

```js
  const countries = ['Estonia', 'Finland', 'Sweden', 'Denmark', 'Norway', 'IceLand'];
  const names = ['Asabeneh', 'Mathias', 'Elias', 'Brook'];
  const numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
```

1. Explain the difference between ***forEach, map, filter, and reduce***.
2. Define a call function before you them in forEach, map, filter or reduce.
3. Use ***forEach*** to console.log each country in the countries array.
4. Use ***forEach*** to console.log each name in the names array.
5. Use ***forEach*** to console.log each number in the numbers array.
6. Use ***map*** to create a new array  by changing each country to uppercase in the countries array;
7. Use ***map*** to create a new array  by changing each number to square in the numbers array
8. Use ***map*** to change to each name to uppercase in the names array
9. Use ***filter*** to filter out countries containing ***land***.
10. Use ***filter*** to filter out countries having six character.
11. Use ***filter*** to filter out countries containing six letters and more in the country array.
12. Use ***filter*** to filter out country start with 'E';
13. Chain two or more array iterators(eg. arr.map(callback).filter(callback).reduce(callback))
14. Declare a function called getStringLists which takes an array as a parameter and then returns an array only with string items.
15. Use ***reduce*** to sum all the numbers in the numbers array.
16. Use ***reduce*** to concatenate all the countries and to produce this sentence: ***Estonia, Finland, Sweden, Denmark, Norway, and IceLand are north European countries***
17. Explain the difference between ***some*** and ***every***
18. Use ***some*** to check if some names' length greater than seven in names array
19. Use ***every*** to check if all the countries contain the word land
20. Explain the difference between ***find*** and ***findIndex***.
21. Use ***find*** to find the first country containing only six letters in the countries array
22. Use ***findIndex*** to find the position of the first country containing only six letters in the countries array
23. Use ***findIndex*** to find the position of ***Norway*** if it doesn't exist in the array you will get -1.
24. Use ***findIndex*** to find the position of ***Russia*** if it doesn't exist in the array you will get -1.
25. Declare a function called ***categorizeCountries*** which returns an array of countries which have some common pattern(you find the countries array in this repository as countries.js(eg 'land', 'ia', 'island','stan')).
26. Create a function which return an array of objects, which is the letter and the number of times the letter use to start with a name of a country.
27. Declare a ***getFirstTenCountries*** function and return an array of ten countries. Use different functional programming to work on the countries.js array
28. Declare a ***getLastTenCountries*** function which which returns the last ten countries in the countries array.
29. Find out which *letter* is used many *times* as initial for a country name from the countries array (eg. Finland, Fiji, France etc)
30. Use the countries information, in the data folder. Sort countries by name, by capital, by population
31. Sort out the ten most spoken languages by location.
32. Sort out the ten most populated countries.

## Destructuring and Spread

Destructuring is a way to unpack arrays, and objects and assigning to a distinct variable.

### Destructing  Arrays

```js
  const numbers = [1, 2,3];
  let [numOne, numTwo, numThree] = numbers;
  console.log(numOne, numTwo, numThree) // 1,2,3
  const names = ['Asabeneh', 'Brook', 'David', 'John']
  let [firstPerson, secondPerson, ThirdPerson, fourth Person] = names;
  console.log(firstName, secondPerson,thirdPerson, fourthPerson) //Asabeneh, Brook, David, John
  const scientificConstants = [2.72, 3.14, 9.81, 37, 100];
  let [e, pi, gravity, bodyTemp, boilingTemp] = scientificConstants
  console.log(e,pi,gravity, bodyTemp, boilingTemp) //2.72, 3.14, 9.81, 37, 100
```

If we like to skip on of the values in the array we use additional comma. The comma helps to omit the value at that index

```js
  const numbers = [1, 2,3];
  let [numOne, , , numThree] = numbers; //2 is omitted
  console.log(numOne,, numThree) // 1,2,3
  const names = ['Asabeneh', 'Brook', 'David', 'John']
  let [, secondPerson, , fourth Person] = name; // first and third person is omitted
  console.log(secondPerson, fourthPerson) //Brook, John
```

We can use default value in case the value of array for that index is undefined:

```js
const names = [undefined, 'Brook', 'David'];
let [firstPerson = 'Asabeneh', secondPerson, thirdPerson, fourthPerson = 'John' ] = names;
console.log(firstPerson, secondPerson, thirdPerson, fourthPerson) // Asabeneh Brook David John
```

#### Destructuring Object

When we destructure the name of the variable we use to destructure should be exactly the same us the key or property of the object. See example below.

```js
const rectangle = {
  width: 20,
  height:10,
  area: 200
}
let {width, height, area, perimeter} = rectangle;
console.log(width, height, area, perimeter) //20 10 200 undefined
```

#### Renaming during structuring

```js
const rectangle = {
  width: 20,
  height:10,
  area: 200
}
let {width:w, heigh:h, area:a, perimeter:p} = rectangle;
console.log(w, h, a, p) //20 10 200 undefined
```

If the key is not found in the object the variable will be assigned to undefined. In case, the key is not in the object we can give a default value during declaration. See the example.

```js
const rectangle = {
  width: 20,
  height:10,
  area: 200
}
let {width, heigh, area, perimeter = 60} = rectangle;
console.log(width, height, area, perimeter)  //20 10 200 60

//Lets modify the object:width to 30 and perimeter to 80
const rectangle = {
  width: 30,
  height:10,
  area: 200,
  perimeter:80
}
let {width, heigh, area, perimeter = 60} = rectangle;
console.log(width, height, area, perimeter) //20 10 200 80
```

Destructuring keys as a function parameters. Lets create a function which take a rectangle object and it return a perimeter of a rectangle.

```js
    // Without destructuring
    const rect = {
      width:20,
      height:10
    }
    const calculatePerimeter = (rectangle) => {
      return 2 * (rectangle.width + rectangle.height)
    }
    console.log(calculatePerimeter(rect)) // 60
    //with destructuring

     const calculatePerimeter = ({width, height}) => {
      return 2 * (width + height)
    }

    console.log(calculatePerimeter(rect)) // 60

    //Another Example
const person = {
  firstName: 'Asabeneh',
  lastName: 'Yetayeh',
  age: 200,
  country: 'Finland',
  job: 'Instructor and Developer',
  skills: [
    'HTML',
    'CSS',
    'JavaScript',
    'React',
    'Redux',
    'Node',
    'MongoDB',
    'Python',
    'D3.js'
  ],
  languages: ['Amharic', 'English', 'Suomi(Finnish)']
};
// Lets create a function which give information about the person object without destructuring

const getPersonInfo = obj => {
  const skills = obj.skills;
  const formattedSkills = skills.slice(0, -1).join(', ');
  const languages = obj.languages;
  const formattedLanguages = languages.slice(0, -1).join(', ');

  return `${obj.firstName} ${obj.lastName} lives in ${obj.country}. He is  ${
    obj.age
  } years old. He is an ${obj.job}. He teaches ${formattedSkills} and ${
    skills[skills.length - 1]
  }. He speaks ${formattedLanguages} and a little bit of ${languages[2]}.`;
};
console.log(getPersonInfo(person));
// Lets create a function which give information about the person object with destructuring

const getPersonInfo = ({
  firstName,
  lastName,
  age,
  country,
  job,
  skills,
  languages
}) => {
  const formattedSkills = skills.slice(0, -1).join(', ');
  const formattedLanguages = languages.slice(0, -1).join(', ');

  return `${firstName} ${lastName} lives in ${country}. He is ${age} years old. He is an ${job}. He teaches ${formattedSkills} and ${skills[skills.length - 1]}. He speaks ${formattedLanguages} and a little bit of ${languages[2]}.`;
};
console.log(getPersonInfo(person))
/*
Asabeneh Yetayeh lives in Finland. He is  200 years old. He is an Instructor and Developer. He teaches HTML, CSS, JavaScript, React, Redux, Node, MongoDB, Python and D3.js. He speaks Amharic, English and a little bit of Suomi(Finnish)
*/
```

### Spread or Rest Operator

#### Exercise: Destructuring

   ```js
   const constants = [2.72, 3.14, 9.81,37, 100]
   const countries = ['Finland', 'Estonia', 'Sweden', 'Denmark', 'Norway']

   const rectangle = {
     width:20,
     height:10,
     area:200,
     perimeter:60
   }
   ```

   1. Assign the elements of constants array to e, pi, gravity, humanBodyTemp, waterBoilingTemp.
   2. Assign the elements of countries array to fin, est, sw, den, nor
   3. Destructure the rectangle object by its properties or keys.

## Map and Set

## Set

Set is a collection of unique elements. Lets see how to create a set

### Creating a set

```js
  const companies = new Set()
```

### Adding an element to a set

```js
  console.log(companies.size) // 0
  companies.add('Google') // add element to the set
  companies.add('Facebook')
  companies.add('Amazon')
  companies.add('Oracle')
  companies.add('Microsoft')
  console.log(companies.size) // 5 elements in the set
```

### Deleting an element a set

```js
console.log(companies.delete('Google'))
console.log(companies.size) // 4 elements left in the set
```

### Checking an element in the set

```js
console.log(companies.has('Google')) // false
console.log(companies.has('Facebook')) // true
```

### Clearing the set

It removes all the elements

```js
  companies.clear()
```

See the example below to learn how to use set.

```js

const languages = [
  'English',
  'Finnish',
  'English',
  'French',
  'Spanish',
  'English',
  'French'
]
const langSet = new Set(languages)
console.log(langSet)
console.log(langSet.size)

const counts = []
const count = {}

for (const l of langSet) {
  const filteredLang = languages.filter(lng => lng === l)
  console.log(filteredLang)
  counts.push({ lang: l, count: filteredLang.length })
}
console.log(counts)
```

## Map

### Creating a Map

```js
  const countriesMap = new Map()
```

### Adding values to the Map

```js
  console.log(countriesMap.size)
  countriesMap.set('Finland', 'Helsinki')
  countriesMap.set('Estonia', 'Tallinn')
  countriesMap.set('Sweden', 'Stockholm')
  console.log(countriesMap)
  console.log(countriesMap.size)
```

### Getting a value from Map

```js
  console.log(countriesMap.get('Finland'))
```

### Checking key in Map

```js
 console.log(countriesMap.has('Finland'))
```

Getting all values from map using loop

```js
  for (const cnt of countriesMap) {
    console.log(cnt)
  }
  ```

## Document Object Model (DOM)

HTML document is structured as a JavaScript Object. Every HTML element has a different properties which can help to manipulate it. It is possible to get, create, append or remove HTML elements using JavaScript. Check the examples below. Selecting HTML element using JavaScript is similar to select CSS. To select an HTML element, we use tag name, id, class name. To create an HTML element we use tag name.

### Getting Element

```html
<!DOCTYPE html>
  <html>
    <head>
      <title>Document Object Model/title>
    </head>
    <body>
     <h1 class='title' id='first-title'>First Title</h1>
     <h1 class='title' id='second-title'>Second Title</h1>
     <h1 class='title' id='third-title'>Third Title</h1>
     <h1></h1>
    </body>
  </html>
```

#### Getting elements by tag name

***getElementsByTagName()*** method returns an HTMLCollection object. An HTMLCollection is an array like list of HTML elements. The length property provides the size of the collection.

```js
const allTitles = document.getElementsByTagName('h1');
console.log(allTitles) //HTMCollections
console.log(allTitles.length) // 4
for(let i = 0; i < allTitles.length; i++){
  console.log(allTitles[i]) // prints each elements in the HTMLCollection
}
```

#### Getting elements by class name

***getElementsByClassName()*** method returns an HTMLCollection object. An HTMLCollection is an array like list of HTML elements. The length property provides the size of the collection. It is possible to loop through all the HTMLCollection elements. See the example below

```js
const allTitles = document.getElementsByClassName('title');
console.log(allTitles) //HTMCollections
console.log(allTitles.length) // 4
for(let i = 0; i < allTitles.length; i++){
  console.log(allTitles[i]) // prints each elements in the HTMLCollection
}
```

#### Getting an element by id

***getElementsById()***  targets a single HTML element. We pass the id without # as an argument.

```js
let firstTitle = document.getElementById('first-title');
console.log(firstTitle) // <h1>First Title</h1>
```

#### Getting elements by using querySelector using tag, class and id:

***querySelector***: can be used to select HTML element by its tag name, id or class. If the tag name is used it selects only the first element.

```js
let firstTitle = document.querySelect('h1');// select the first available h2 element
let firstTitle = document.querySelector('#first-title'); // select id with first-title
let firstTitle = document.querySelector('.title'); // select the first available h2 element with class title
```

***querySelectorAll***: can be used to select html element by its tag name or class. It return a nodeList which is an array like object which support array methods. We can use ***for loop*** or ***forEach*** to loop through each nodeList elements.

```js
const allTitles = document.querySelectAll('h1');
console.log(allTitles.length) // 4
for(let i = 0; i < allTitles.length; i++){
  console.log(allTitles[i]);
}
allTitles.forEach(title => console.log(title))
const allTitles = document.querySelectorAll('.title'); // the same goes for selecting using class
```

### Adding attribute

An attribute is added in the opening tag of HTML which gives additional information about the element. Common HTML attributes: id, class, src, style, href,disabled, title, alt. Lets add id and class for the fourth title.

#### Adding attribute using setAttribute

The ***setAttribute()*** method set any html attribute. It takes two parameters the type of the attribute and the name of the attribute. 
Let's add class and id attribute for the fourth title.

```js
const titles = document.querySelectorAll('h1');
titles[3].setAttribute('class', 'title');
titles[3].setAttribute('id', 'fourth-title');
```

#### Adding attribute without setAttribute

Some attributes are DOM object property and they can be set directly. For instance id and class

```js
//another way to setting an attribute
titles[3].className = 'title';
titles[3].id = 'fourth-title';
```

#### Adding class using classList

The class list method is a good method to append additional class. It doesn't override the original class if a class exists

```js
//another way to setting an attribute: append the class, doesn't over ride
titles[3].classList.add('title', 'header-title')
```

### Adding Text content

```js
const titles = document.querySelectorAll('h1');
titles[3].textContent = 'Fourth Title';
```

### Adding style

Lets add some style to our titles. If the element has even index we give it green color else red.

```js
const titles = document.querySelectorAll('h1');
titles.forEach((title,i) => {
  title.fontSize = '24px'; // all titles will have 24px font size
  if(i % 2 === 0){
    title.style.color = 'green';
  }
  else {
    title.style.color = 'red';
  }
})

```

### Creating an Element

```js
let title = document.createElement('h1');
let firstTitle = document.getElementById('first-title');
```

### Creating elements

```js
let firstTitle = document.getElementById('first-title');
let title
for(let i = 0; i < 3; i++){
  title = document.createElement('h1');
  title.className = 'title';
  title.style.fontSize = '24px';
}
```

### Appending to a parent element

```js
// creating multiple elements and appending to parent element
let title;
for(let i = 0; i < 3; i++){
  title = document.createElement('h1');
  title.className = 'title';
  title.style.fontSize = '24px';
  document.body.appendChild(title);
}
```

### Event Listeners

Common HTML events:onclick, onchange, onmouseover, onmouseout, onkeydown, onkeyup, onload.
We can add event listener method to any DOM object. Use use ***addEventListener()*** method to listen different event types on HTML elements.
The following is an example of click type event.

```js
const button = document.querySelector('button');
button.addEventListener('click', e => {
  console.log(e.target);
});
```

### Getting value from an input element

We usually fill forms and forms accept data. Form fields are created using input HTML element.

```html
<input type ='text' placeholder = 'Mass in Kilogram' />
<input type = 'text' placeholder = 'Height in meters' />
<button>Calculate BMI</button>
```

```js
const mass = document.querySelector('#mass');
const height = document.querySelector('#height');
const button = document.querySelector('button');
let bmi;
button.addEventListen('click', ()=>{
  bmi = mass.value * height.value;
});

console.log(bmi)
```

#### Exercises:Document Object Model

```html
  <!-- index.html -->
<!DOCTYPE html>
  <html>
    <head>
      <title>JavaScript for Everyone:DOM</title>
    </head>
    <body>
    <p>First Paragraph</p>
    <p>Second Paragraph</p>
    <p>Third Paragraph</p>
    <p></p>
    </body>
  </html>
```

  1. Create an index.html file and put four p elements as above: Get the first paragraph by using ***document.querySelector(tagname)*** and tag name
  2. Get get each of the the paragraph using ***document.querySelector('#id')*** and by their id
  3. Get all the p as nodeList using ***document.querySelectorAll(tagname)*** and by their tag name
  4. Loop through the nodeList and get the text content of each paragraph
  5. Set a text content to paragraph the fourth paragraph,***Fourth Paragraph***
  6. Set id and class attribute for all the paragraphs using different attribute setting methods
  7. Change stye of each paragraph using JavaScript(eg. color, background, border, font-size, font-family)
  8. Select all paragraphs and loop through each elements and give the first and third paragraph a color of color, and the second and the fourth paragraph a red color
  9. Remove all the paragraph and create them using JavaScript
  10. Set text content, id and class to each paragraph
  11. Create a div container on HTML document and create 100 numbers dynamically and append to the container div. Put each number in 150px by 150px box. If the number is even the background will be lightgreen else lightblue.
  12. Use the rgb color generator function or hexaColor generator to create 10 divs with random background colors
  13. Use the countries.js to visualize all the countries on the HTML document. You need one wrapper div and box for each countries. In the box display, the letter the country starts with, the name of the country and the number of characters for the country name.

#### DOM: Mini Projects

1. BMI calculator
2. Hexadecimal or RGB color Generator
3. World Countries List

## Class

```js
class Person {
  constructor(firstName, lastName, age, location, skills) {
    this.firstName = firstName;
    this.lastName = lastName;
    this.age = age;
    this.location = location;
    this.skills = skills;
  }
  getFull() {
    return `${this.firstName} ${this.lastName}`;
  }
}
```

### Exercises:Classes

## Regular Expressions

Regular expression is a small program language which is used with many programming languages. Regular expression match or search for a pattern. We use ' or '' to create a string data type. We can create a pattern in two ways.

### Creating a pattern

```js
let pattern = /love/; 
let pattern = new RegEx('love');
```

### Creating a pattern with flags: global flag (g), case insensitive flag(i)

```js
let pattern = /love/gi; // declaring a regex pattern
let pattern = new RegEx('love','gi');  // declaring a regex pattern using RegEx object
```

```js
let pattern = /[A-Z][a-z]{3,12}/;
let name = 'Asabeneh';
pattern.test(name);
//output:true
```

### RegExp Object Methods

```js
const str = 'I love JavaScript';
const pattern = /love/;
const result = pattern.test(str);
console.log(result);
```

#### Exercises:Regular Expressions

- Calculate the total annual income of the person from the following text. ‘He earns 4000 euro from salary per month, 10000 euro annual bonus, 5500 euro online courses per month.’

## Promises and Callbacks

From the following code blocks you will notice, the difference between callback and promises:

  ```js
      //Callback
    const doSomething = callback => {
    setTimeout(() => {
      const skills = ['HTML', 'CSS', 'JS']
      callback('It didnt go well', skills)
    }, 2000)
  }

  doSomething((err, result) => {
    if (err) {
      return console.log(err)
    }
    return console.log(result)
  })
  // after 2 seconds it will print
  // => It didnt go well

    const doSomething = callback => {
    setTimeout(() => {
      const skills = ['HTML', 'CSS', 'JS']
      callback(false, skills)
    }, 2000)
  }

  doSomething((err, result) => {
    if (err) {
      return console.log(err)
    }
    return console.log(result)
  })
  // after 2 seconds it will print the skills
  // => ["HTML", "CSS", "JS"]

  ```

  ```js
   // Promise
    const doPromise = new Promise((resolve, reject) => {
  setTimeout(() => {
    const skills = ['HTML', 'CSS', 'JS']
    if (skills.length > 0) {
      resolve(skills)
    } else {
      reject('Something wrong has happened')
    }
  }, 2000)
})

doPromise
  .then(result => {
    console.log(result)
  })
  .catch(error => console.log(error))

const myPromise = n => {
  return new Promise((resolve, reject) => {
    if (n) {
      resolve(n * n)
    } else {
      reject('You need to pass an argument')
    }
  })
}

const square = async n => {
  let value = await myPromise(n)
  return value
}

square()
  .then(res => {
    console.log(res)
  })
  .catch(err => console.log(err))
console.log(square(10))
 ```

## Async and Await

```js
    const url = 'https://restcountries.eu/rest/v2/alll'
  fetch(url)
    .then(response => response.json())
    .then(data => {
      console.log(data)
    })
    .catch(error => console.log(error))

  const fetchData = async () => {
    try {
      const response = await fetch(url)
      const countries = await response.json()
      console.log(countries)
    } catch (err) {
      console.log(err)
    }
  }
  console.log('===== async and await')
  fetchData()
  ```

## localStorage

Local storage is the para of the web storage API which is used to store data on the browser with no expiration data. The data will be available on the browser even after the browser is closed. There are five methods to work on local storage:
_setItem(), getItem(), removeItem(), clear(), key()_

### Setting item to the localStorage

When we set data to be stored in a localStorage, it will be stored as a string.  If we are storing an array or an object, we should stringify it first to keep the format unless otherwise we lose the array structure or the object structure of the original data

```js
localStorage.setItem('name', 'Asabeneh');
console.log(localStorage) //Storage {name: 'Asabeneh', length: 1}
localStorage.setItem('age', 200);
console.log(localStorage) //Storage {age: '200', name: 'Asabeneh', length: 2}
const skills = ['HTML', 'CSS', 'JS', 'React'];
//Skills array has to be stringified first to keep the format.
const skillsJSON = JSON.stringify(skills,undefined, 4)
localStorage.setItem('skills', skillsJSON);
console.log(localStorage) //Storage {age: '200', name: 'Asabeneh', skills: 'HTML,CSS,JS,React', length: 3}
```

If we are storing an array, an object or object array, we should stringify the object first. See the example below.

```js
let skills = [
  { tech: 'HTML', level: 10 },
  { tech: 'CSS', level: 9 },
  { tech: 'JS', level: 8 },
  { tech: 'React', level: 9 },
  { tech: 'Redux', level: 10 },
  { tech: 'Node', level: 8 },
  { tech: 'MongoDB', level: 8 }
];

let skillJSON = JSON.stringify(skills);
localStorage.setItem('skills', skillJSON);
```

### Getting item from localStorage

```js
let name = localStorage.getItem('name');
let age = localStorage.getItem('age');
let skills = localStorage.getItem('skills');

console.log(name, age, skills) // 'Asabeneh', '200', '['HTML','CSS','JS','React']'

let skillsObj = JSON.parse(localStorage.getItem('skills'), undefined, 4);
console.log(skillsObj);
```

### Clearing the localStorage

The clear method, will clear everything stored in the local storage

```js
localStorage.clear();
```

### Exercises:Local Storage

## Cookies

### Exercises:Cookies

## JavaScript Interview Questions

### [JavaScript Tests](https://github.com/Asabeneh/JavaScript-for-Everyone/wiki/JavaScript-Tests)

### [JavaScript Test 1](https://github.com/Asabeneh/JavaScript-for-Everyone/wiki/JavaScript-Test-1)

### [JavaScript Test 2](https://github.com/Asabeneh/JavaScript-for-Everyone/wiki/JavaScript-Test-2)

### [JavaScript Test 3](https://github.com/Asabeneh/JavaScript-for-Everyone/wiki/JavaScript-Test-3)

- [JavaScript Test 3: Solutions](https://github.com/Asabeneh/JavaScript-for-Everyone/blob/master/solutions/javascript-test-3.js)
JavaScript-Test-4)
- [JavaScript Test 4: Solutions](https://github.com/Asabeneh/JavaScript-for-Everyone/blob/master/solutions/javascript-test-4.js)
