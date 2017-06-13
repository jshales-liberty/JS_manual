# My JS Manual

**Welcome to JS**

Write a reference manual for the Javascript language. For each of the following topics, provide a description and (where applicable) a simple example:

- values, data types
- operations / operators / operands
- variables, var
- reserved words
- statements vs. expressions
- variables vs. values

## if-else

- Conditional statement where a certain block of code will be executed if the condition is true otherwise the code block specified by the else is executed.

```
if (hour < 18) {
  greeting = "Good day";
} else {
  greeting = "Good evening";
}
```

## while

- Loops through a block of code as long as a specified condition is true.
```
while (i < cars.length) {
    text += cars[i] + "<br>";
    i++;
}

```

## for

- Loops through a block of code a number of times

```
for (i = 0; i < cars.length; i++) {
    text += cars[i] + "<br>";
 }
```

## for-in

- Loops through the properties of an object

```
var person = {fname:"John", lname:"Doe", age:25};
 var text = "";
var x;
for (x in person) {
    text += person[x];
 }
```
## functions

- A block of code designed to perform a particular task. The function code block will execute when invoked or called. The function can have parameters and the argument values passed into those parameters act as local variables inside the code block. Functions are useful for code reuse and also to have one piece of code produce different results from different arguments.

```
function myFunction(p1, p2) {
    return p1 * p2;              // The function returns the product of p1 and p2
 }
```

## local vs. global variables

- The scope of a variable is the portion of code for which the variable's name has meaning or is said to be visible. Variables declared within a function are local and only accessible within that function or by functions inside that function. Any variables declared outside of a function are considered global.

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

##values, data types
###Primitive values

- Boolean type true or false;
- Null type; Undefined type;
- Number type = 5;
- String type "This is a string";
- Symbol type;
- Objects (datatype) var x = {firstName:"John", lastName:"Doe"};    // Object

###Data types are dynamic and can hold different types

`var x;   			//Now x is undefined`
`var x = 5;         // Now x is a Number`
`var x = "John";     // Now x is a String`

* if adding number data type to a string javascript will treat the number data type as a string. (Automatic type conversion)

## operations / operators / operands
`= is an assignment x = x + 5;``
`+ is and addition operator`
`+	Addition`
`-	Subtraction`
`*	Multiplication`
`/	Division'
`%	Modulus`
`++	Increment`
`--	Decrement`

###= Assignment Operators

`x = y`
`+=	x += y	x = x + y`
`-=	x -= y	x = x - y`
`*=	x *= y	x = x * y`
`/=	x /= y	x = x / y`
`%=	x %= y	x = x % y`

### Comparison Operators

`==	equal to`
`===	equal value and equal type`
`!=	not equal`
`!==	not equal value or not equal type`
`>	greater than`
`<	less than`
`>=	greater than or equal to`
`<=	less than or equal to`
`?	ternary operator`

### Logical Operators`
`&&	logical and`
`||	logical or`
`!	logical not`
### Type Operators`
`typeof	Returns the type of a variable`
`instanceof	Returns true if an object is an instance of an object type`

### Bitwise Operators
`&	AND	5 & 1	0101 & 0001	0001	 1`
`|	OR	5 | 1	0101 | 0001	0101	 5`
`~	NOT	~ 5	 ~0101	1010	 10`
`^	XOR	5 ^ 1	0101 ^ 0001	0100	 4`
`<<	Zero fill left shift	5 << 1	0101 << 1	1010	 10`
`>>	Signed right shift	5 >> 1	0101 >> 1	0010	  2`
`>>>	Zero fill right shift	5 >>> 1	0101 >>> 1	0010	  2`

##variables, var

-All JavaScript variables must be identified with unique names.
-These unique names are called identifiers.
-Identifiers can be short names (like x and y) or more descriptive names (age, sum, totalVolume).
-The general rules for constructing names for variables (unique identifiers) are:
-Names can contain letters, digits, underscores, and dollar signs.
-Names must begin with a letter
-Names can also begin with $
-Names are case sensitive (y and Y are different variables)

##reserved words
*In JavaScript you cannot use these reserved words as variables, labels, or function names:
`abstract	arguments	await*	boolean`
`break	byte	case	catch`
`char	class*	const	continue`
`debugger	default	delete	do`
`double	else	enum*	eval`
`export*	extends*	false	final`
`finally	float	for	function`
`goto	if	implements	import*`
`in	instanceof	int	interface`
`let*	long	native	new`
`null	package	private	protected`
`public	return	short	static`
`super*	switch	synchronized	this`
`throw	throws	transient	true`
`try	typeof	var	void`
`volatile	while	with	yield`
##statements vs. expressions
*An expression produces a value and can be written wherever a value is expected.`
`Every syntactically valid expression resolves to some value but conceptually, there are two types of expressions: with side effects (for example: those that `
`assign value to a variable) and those that in some sense evaluates and therefore resolves to value.`
`The expression x = 7 is an example of the first type. This expression uses the = operator to assign the value seven to the variable x. The expression itself evaluates to seven.`
`The code 3 + 4 is an example of the second expression type. This expression uses the + operator to add three and four together without assigning the result, seven, to a variable.`
`JavaScript has the following expression categories:`

`Arithmetic: evaluates to a number, for example 3.14159. (Generally uses arithmetic operators.)`
`String: evaluates to a character string, for example, "Fred" or "234". (Generally uses string operators.)`
`Logical: evaluates to true or false. (Often involves logical operators.)`
`Primary expressions: Basic keywords and general expressions in JavaScript.`
`Left-hand-side expressions: Left values are the destination of an assignment.`
*A statement performs an action. Loops and if statements are examples of statements`
*Statements are executed, one by one, in the same order as they are written.`
*Statements end with semicolon.
`var a, b, c;`
`a = 5;`
`b = 6;`
`c = a + b;`
##variables vs. values
-variables store a refrence to a value. 
-values can be assigned to variables.
`example of variable assigned a value:  var x = 9;`


- All JavaScript variables must be identified with unique names.
- These unique names are called identifiers.
- Identifiers can be short names (like x and y) or more descriptive names (age, sum, totalVolume).
- The general rules for constructing names for variables (unique identifiers) are:
- Names can contain letters, digits, underscores, and dollar signs.
- Names must begin with a letter
- Names can also begin with $
- Names are case sensitive (y and Y are different variables)


if-else
while
for
for-in
functions
local vs. global variables

## arrays

a collection of variables stored contiguously in memory, able to be referenced by indices. Arrays can contain different types of variables, meaning a given array could contain both strings and ints for example.

```var a = [1,5,"abc"];```

## objects

objects in JS are variables that contain many values in the form of named value pairs. Objects are instantiated, meaning a given object is created and obeys a previously defined structure. For each named property of an object the property can be adjusted by referencing it with [], similar to how one might reference a given index of an array. Objects have no concept of order in how their data in stored. Objects also have the special "this" keyword that can reference values specific to that instance of the object.

```var cat1 = new Object();
cat1["whiskers"] = 9;
cat1["name"]=Tobin;
```

## methods

*methods are functions contained as values within an object. these functions can be called on an instance of that object. Methods are called using dot notation on an instance of an object.*

```cat1.purr() //for instance this may print a purring noise to the console
cat1.eat() //this might increment the weight of the cat
```
## the different uses of . [] {} ;

for .
-	accessing/calling methods
-	accessing/assigning properties of objects

for []
-	creating an array []
-	assign array to a variable: var a = [2,3];
-	access/assign to index of arrays: a[0] = 3
-	access/assign to key of object o["key"] = 4;

for {}
-	body of function, loops, ifelse,
-	compound statements
-	create an object {foo: 3, "hi": 2}

for ;
- end statement without {} body
-	seperates for loop syntax (pre condition; condition; post-condition)

for ()

-	surround conditions of if statement if (true)...
-	calling a function foo()
-	control order of operations (2+3)/2
-	surround parameters

## object links

**an object link takes you to a different part of the html page when clicked on/triggered in JavaScript**

## anonymous functions

**annonymous functions are functions that are defined without a name and are typically only called once. for instance, when setting up an event handler one might put an annonymous function the action triggered when the event is triggered. annonymous functions can be good tools if one can't think of a good thing to call a process that should really only exist at one place in one's code.**

```
///here's an example of an annonymous function in my pong game event listener
	window.addEventListener("keydown", function(evt) {var key = evt.keyCode; console.log(key);
		switch(key)
		{case 38:right_rect.top-=6; break;
		case 40:right_rect.top+=6; break;
		case 65:left_rect.top-=6; break;
		case 90:left_rect.top+=6; break;
		}
```

## nested function scope / closures

**Variables can be defined globally (accesible to all parts of your code) or locally (contained and accesible only within a given function). All functions have access to the scope "one above them" meaning most functions have access to the global scope but if you were to define a function within a function (nesting that function) the nested function would have have access to variables one function up (not in the global space).**

## exceptions

* Thrown during runtime, can be a built in exception or a custom one created by the developer.  Shouldn't be used to control flow but should be handled.

## try-catch

* Used to surround a block of code that may throw an error at runtime.  Generally not used to control flow. The try is the code you want to execute, and the catch is used to handle the error.  It can be used to throw the error from the language or define and throw a custom error.

```
try {
  document.getElementById("addressLine2");
} catch (err) {
  alert("element not found");
}
```

## the global namespace

* Objects / variables in the global namespace have global scope, so they are available to the entire code.  This includes functions and types.

## important functions and objects in the global namespace

* The objects upon which all other objects are built, the standard language features.  These include:

```
Function
Error
Object
```
## DOM methods and properties

* mechanism for the javascript / ecmascript code to interact with the HTML page, allows you to traverse the HTML tree, retrieve and change specific nodes, react to events.

## event handlers

* An event is an action on the page within the browser, and the handler is the code that is triggered when that event occurs.  For example, onload, onclick, hover all are events that are exposed to allow you to write code in response to those events.
