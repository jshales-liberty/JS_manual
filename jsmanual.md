# My JS Manual

**Welcome to JS**

Write a reference manual for the Javascript language. For each of the following topics, provide a description and (where applicable) a simple example:

##values, data types 
###Primitive values
	*Boolean type true or false; 
	*Null type; Undefined type; 
	*Number type = 5; 
	*String type "This is a string"; 
	*Symbol type; 
	`Objects (datatype) var x = {firstName:"John", lastName:"Doe"};    // Object
###Data types are dynamic and can hold different types 
`var x;   			//Now x is undefined
`var x = 5;         // Now x is a Number
`var x = "John";     // Now x is a String
* if adding number data type to a string javascript will treat the number data type as a string. (Automatic type conversion)
##operations / operators / operands
`= is an assignment x = x + 5;
`+ is and addition operator 
`+	Addition
`-	Subtraction
`*	Multiplication
`/	Division'
`%	Modulus
`++	Increment
`--	Decrement
###= Assignment Operators
`x = y
`+=	x += y	x = x + y
`-=	x -= y	x = x - y
`*=	x *= y	x = x * y
`/=	x /= y	x = x / y
`%=	x %= y	x = x % y
### Comparison Operators
`==	equal to
`===	equal value and equal type
`!=	not equal
`!==	not equal value or not equal type
`>	greater than
`<	less than
`>=	greater than or equal to
`<=	less than or equal to
`?	ternary operator
### Logical Operators
`&&	logical and
`||	logical or
`!	logical not
### Type Operators
`typeof	Returns the type of a variable
`instanceof	Returns true if an object is an instance of an object type
### Bitwise Operators
`&	AND	5 & 1	0101 & 0001	0001	 1
`|	OR	5 | 1	0101 | 0001	0101	 5
`~	NOT	~ 5	 ~0101	1010	 10
`^	XOR	5 ^ 1	0101 ^ 0001	0100	 4
`<<	Zero fill left shift	5 << 1	0101 << 1	1010	 10
`>>	Signed right shift	5 >> 1	0101 >> 1	0010	  2
`>>>	Zero fill right shift	5 >>> 1	0101 >>> 1	0010	  2

##variables, var
*All JavaScript variables must be identified with unique names.
*These unique names are called identifiers.
*Identifiers can be short names (like x and y) or more descriptive names (age, sum, totalVolume).
*The general rules for constructing names for variables (unique identifiers) are:
*Names can contain letters, digits, underscores, and dollar signs.
*Names must begin with a letter
*Names can also begin with $
*Names are case sensitive (y and Y are different variables)

##reserved words
*In JavaScript you cannot use these reserved words as variables, labels, or function names:
'abstract	arguments	await*	boolean
'break	byte	case	catch
'char	class*	const	continue
'debugger	default	delete	do
'double	else	enum*	eval
'export*	extends*	false	final
'finally	float	for	function
'goto	if	implements	import*
'in	instanceof	int	interface
'let*	long	native	new
'null	package	private	protected
'public	return	short	static
'super*	switch	synchronized	this
'throw	throws	transient	true
'try	typeof	var	void
'volatile	while	with	yield
##statements vs. expressions
*An expression produces a value and can be written wherever a value is expected.
*Astatement performs an action. Loops and if statements are examples of statements
##variables vs. values
if-else
while
for
for-in
functions
local vs. global variables
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
## exceptions
* definition
## try-catch
* Used to surround a block of code that may throw an error at runtime.  
Generally not used to control flow. The try is the code you want to execute, and the
catch is used to handle the error.  It can be used to throw the error from the language
or define and throw a custom error.
```
try catch example
```
## the global namespace
* definition
## important functions and objects in the global namespace
* definition
## DOM methods and properties
* definition
## event handlers
* definition
