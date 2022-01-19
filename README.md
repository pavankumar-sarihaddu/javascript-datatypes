# javascript-datatypes
In programming, data types is an important concept.  To be able to operate on variables, it is important to know something about the type.
Without data types, a computer cannot safely solve this:

let x = 16 + "Volvo";
Does it make any sense to add "Volvo" to sixteen? Will it produce an error or will it produce a result?

JavaScript will treat the example above as:

let x = "16" + "Volvo";
When adding a number and a string, JavaScript will treat the number as a string.
JavaScript evaluates expressions from left to right. Different sequences can produce different results:
JavaScript:
let x = 16 + 4 + "Volvo";
Result: 20Volvo
JavaScript:
let x = "Volvo" + 16 + 4;
Result:  Volvo164.

In the first example, JavaScript treats 16 and 4 as numbers, until it reaches "Volvo".

In the second example, since the first operand is a string, all operands are treated as strings.
JavaScript Types are Dynamic
JavaScript has dynamic types. This means that the same variable can be used to hold different data types:
let x;           // Now x is undefined
x = 5;           // Now x is a Number
x = "John";      // Now x is a String
JavaScript Strings
A string (or a text string) is a series of characters like "John Doe".

Strings are written with quotes. You can use single or double quotes:
Example
let carName1 = "Volvo XC60";   // Using double quotes
let carName2 = 'Volvo XC60';   // Using single quotes
You can use quotes inside a string, as long as they don't match the quotes surrounding the string:

Example
let answer1 = "It's alright";             // Single quote inside double quotes
let answer2 = "He is called 'Johnny'";    // Single quotes inside double quotes
let answer3 = 'He is called "Johnny"';    // Double quotes inside single quotes

JavaScript Numbers
JavaScript has only one type of numbers.

Numbers can be written with, or without decimals:

Example
let x1 = 34.00;     // Written with decimals
let x2 = 34;        // Written without decimals
Extra large or extra small numbers can be written with scientific (exponential) notation:

Example
let y = 123e5;      // 12300000
let z = 123e-5;     // 0.00123
JavaScript Booleans
Booleans can only have two values: true or false.

Example
let x = 5;
let y = 5;
let z = 6;
(x == y)       // Returns true
(x == z)       // Returns false
JavaScript Arrays
JavaScript arrays are written with square brackets.

Array items are separated by commas.

The following code declares (creates) an array called cars, containing three items (car names):

Example
const cars = ["Saab", "Volvo", "BMW"];
Array indexes are zero-based, which means the first item is [0], second is [1], and so on.
JavaScript Objects
JavaScript objects are written with curly braces {}.

Object properties are written as name:value pairs, separated by commas.

Example
const person = {firstName:"John", lastName:"Doe", age:50, eyeColor:"blue"};
The object (person) in the example above has 4 properties: firstName, lastName, age, and eyeColor.
The typeof Operator
You can use the JavaScript typeof operator to find the type of a JavaScript variable.

The typeof operator returns the type of a variable or an expression:

Example
typeof ""             // Returns "string"
typeof "John"         // Returns "string"
typeof "John Doe"     // Returns "string"
Example
typeof 0              // Returns "number"
typeof 314            // Returns "number"
typeof 3.14           // Returns "number"
typeof (3)            // Returns "number"
typeof (3 + 4)        // Returns "number"
Undefined
In JavaScript, a variable without a value, has the value undefined. The type is also undefined.

Example
let car;    // Value is undefined, type is undefined
Any variable can be emptied, by setting the value to undefined. The type will also be undefined.

Example
car = undefined;    // Value is undefined, type is undefined
Empty Values
An empty value has nothing to do with undefined.

An empty string has both a legal value and a type.

Example
let car = "";    // The value is "", the typeof is "string"
