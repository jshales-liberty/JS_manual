# My JS Manual

**Welcome to JS**

Write a reference manual for the Javascript language. For each of the following topics, provide a description and (where applicable) a simple example:

values, data types
operations / operators / operands
variables, var
reserved words
statements vs. expressions
variables vs. values
## if-else
* Conditional statement where a certain block of code will be executed if the condition is true otherwise the code block specified by the else is executed.
```
if (hour < 18) {
  greeting = "Good day";
} else {
  greeting = "Good evening";
}
```
## while
* Loops through a block of code as long as a specified condition is true.
```
while (i < cars.length) {
    text += cars[i] + "<br>";
    i++;
}
```
## for
* Loops through a block of code a number of times
```
for (i = 0; i < cars.length; i++) {
    text += cars[i] + "<br>";
 }
 ```
## for-in
* Loops through the properties of an object
```
var person = {fname:"John", lname:"Doe", age:25};
 var text = "";
var x;
for (x in person) {
    text += person[x];
 }
 ```
## functions
* A block of code designed to perform a particular task. The function code block will execute when invoked or called. The function can have parameters and the argument values passed into those parameters act as local variables inside the code block. Functions are useful for code reuse and also to have one piece of code produce different results from different arguments.
```
function myFunction(p1, p2) {
    return p1 * p2;              // The function returns the product of p1 and p2
 }
 ```
## local vs. global variables
* The scope of a variable is the portion of code for which the variable's name has meaning or is said to be visible. Variables declared within a function are local and only accessible within that function or by functions inside that function. Any variables declared outside of a function are considered global.
```
//Local variable example:
// code here can not use carName
function myFunction() {
    var carName = "Volvo";
    // code here can use carName
}
//Global variable example:
var carName = " Volvo";
// code here can use carName
function myFunction() {
    // code here can use carName
}
```
arrays
objects
methods
the different uses of . [] {} ;
for .
	accessing/calling methods
	accessing/assigning properties of objects
for []
	creating an array []
	assign array to a variable: var a = [2,3];
	access/assign to index of arrays: a[0] = 3
	access/assign to key of object o["key"] = 4;
for {}
	body of function, loops, ifelse,
	compound statements
	create an object {foo: 3, "hi": 2}
for ;
	end statement without {} body
	seperates for loop syntax (pre condition; condition; post-condition)
for ()
	surround conditions of if statement if (true)...
	calling a function foo()
	control order of operations (2+3)/2
	surround parameters
object links
anonymous functions
nested function scope / closures
exceptions
try-catch
the global namespace
important functions and objects in the global namespace
DOM methods and properties
event handlers
