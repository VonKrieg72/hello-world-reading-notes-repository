# Programming-With-JavaScript

## Expressions and operators

### Operators

The following types of operators exist in JavaScript:

[Assignment Operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators#assignment_operators) This operator designates a value to its left operand which is based on the value of its right operand. *(Mozilla and Individual Contributors, “Expressions and Operators”, 2005-2021)*

[Comparison Operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators#comparison_operators) This operator does a comparison of its operands, and a logical value is returned, which is based upon if the comparison is true or not.*(Mozilla and Individual Contributors, “Expressions and Operators”, 2005-2021)*

[Arithmetic Operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators#arithmetic_operators) Numerical values are taken by this operator (either literals or variables) as their operands and a single numerical value is returned.  

[Bitwise Operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators#bitwise_operators) The operands or this operator is treated as a set of 32 bits (zeros & ones), rather than as a decimal, hexadecimal, or octal numbers. *(Mozilla and Individual Contributors, “Expressions and Operators”, 2005-2021)*

[Logical Operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators#logical_operators) This operator is usually used with Boolean (logical) values; whenever this happens a Boolean value is returned. *(Mozilla and Individual Contributors, “Expressions and Operators”, 2005-2021)*

[String Operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators#string_operators) Along with the comparison operators, which have the ability to be used on string values, the concatenation operator (+) concatenates two string values together, giving back another string that is the co-joining of the two operand strings. *(Mozilla and Individual Contributors, “Expressions and Operators”, 2005-2021)*

[Conditional (ternary) operator](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators#conditional_ternary_operator) This is the only JavaScript operator that takes three operands. The operator has the ability to have one of two values related on a condition. *(Mozilla and Individual Contributors, “Expressions and Operators”, 2005-2021)*

[Comma Operator](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators#comma_operator) This operator (,) takes a look at both of its operands and gives back the value of the last operand. 

[Unary Operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators#unary_operators) This operator is an operation with only one operand. *(Mozilla and Individual Contributors, “Expressions and Operators”, 2005-2021)*

[Relational Operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators#relational_operators) This operator likens its operands and gives back a Boolean value in relation to whether or not the comparison is true. 

*(Mozilla and Individual Contributors, “Expressions and Operators”, 2005-2021)*

### Expressions

An expression is any logical unit of code that resolves to a value. There are two kinds of expressions: with side effects (for example: those that administer value to a variable) and those that kind of evaluate and as a result resolve to a value. JavaScript has the following expression categories:

-Arithmetic: estimates to a number, for example, 9.51413 (Usually uses arithmetic operators)

-String: assesses to a character string, for example, "John" or "483" (Usually uses string operators)

-Logical: assesses to true or false. (In many cases it involves logical operators)

-Primary Expressions: These are general expressions and basic keywords in JavaScript.

-Left-hand-side expressions: Left values are the end of a journey or travel of an assignment.

*(Mozilla and Individual Contributors, “Expressions and Operators”, 2005-2021)*

## Functions

Functions are one of the building blocks that serve as a basis in JavaScript. A function in JavaScript resembles a procedure, which is a set of single declarations or remarks that do a task or determines a value through a mathematical process; however, in order for a procedure to qualify as a function, it should take some input and return an output. 

*(Mozilla and Individual Contributors, “Functions”, 2005-2021)*

### Defining Functions

A **function definition,**which is also known as a function declaration or function statement has the function keyword followed by:

-What the name of the function is.

-An enumeration of the function’s parameters, which are inside parentheses and separated by commas.

-Inside the curly brackets { } are the JavaScript statements, which define the function,. For example, the following code defines a simple function named square:

function square(number) {
  
  return number * number;

}

*(Mozilla and Individual Contributors, “Functions”, 2005-2021)*

### Function Expressions

Functions also have the ability to be created by a function expression. Such a function can be unknown; it doesn't have to have a name. For example, the function square can be defined as:

const square = function(number) { return number * number }

var x = square(4) // x gets the value 16

However, a name can be provided with a function expression.

const factorial = function fac(n) { return n < 2 ? 1 : n * fac(n - 1) }

console.log(factorial(3))

*(Mozilla and Individual Contributors, “Functions”, 2005-2021)*

### Calling functions

Defining a function does not make it do what it has to do (execute). Defining a function gives it a name, and it lets you know exactly what to do (specify) when the function is called. Calling the function actually makes it do the action that it’s supposed to do, with the indicated parameters. For example, if you were to give a definition to the function square, you could call it the following: 

square(5);

The statement above calls the function with an argument of 5. The function does what it’s supposed to do with its statements, and gives you a  value of 25. Functions have to be in scope when they are called; however,  the function declaration has the ability to be hoisted (appear below the call in the code), for example;

console.log(square(5));

/* ... */

function square(n) { return n * n }

*(Mozilla and Individual Contributors, “Functions”, 2005-2021)*

### Function Scope

Variables which are told about in great detail (defined) inside a function can not  be gained access to from anywhere outside the function, because the variable is described in detail (defined) only in the scope of the function; however, a function can reach all variables and functions defined inside the scope in which it is being described in great detail (defined), for example, 

// The variables below are defined in the global scope

var num1 = 20,
    
    num2 = 3,
    
    name = 'Chamakh';

// This function is defined in the global scope

function multiply() {
  
  return num1 * num2;

}

multiply(); // Returns 60

// A nested function example
f
unction getScore() {
  
  var num1 = 2,
      
      num2 = 3;

  function add() {
    
    return name + ' scored ' + (num1 + num2);
  
  }

  return add();

}

getScore(); // Returns "Chamakh scored 5

*(Mozilla and Individual Contributors, “Functions”, 2005-2021)*

### Nested Functions and Closures

You have the ability to nest a function within another function. The nested (inner) function exposes nothing (private) to its containing (outer) function. It also forms a **closure,** which is an expression (most commonly, a function) which can have variables that are free, along with an environment that binds those variables (that closes the expression). Being that a nested function is a closure, this means that a nested function has the ability to "inherit" the arguments and variables of its containing function. In other words, the inner function has inside of it (contains) the scope of the outer function. 

function addSquares(a, b) {
  
  function square(x) {
    
    return x * x;
  
  }
  
  return square(a) + square(b);

}

a = addSquares(2, 3); // returns 13

b = addSquares(3, 4); // returns 25

c = addSquares(4, 5); // returns 41

Since the inner function forms a closure, you can call the outer function and specify arguments for both the outer and inner function.

function outside(x) {
  
  function inside(y) {
    
    return x + y;
 
 }
  
  return inside;

}

fn_inside = outside(3); // Think of it like: give me a function that adds 3 to whatever you g

give
                        // it
result = fn_inside(5); // returns 8

result1 = outside(3)(5); // returns 8

*(Mozilla and Individual Contributors, “Functions”, 2005-2021)*

### Closures

One of the most powerful features of JavaScript is Closures. JavaScript enables the nesting of functions and gives the inner function full access to all the variables and the functions described about in great detail (defined) inside the outer function (and all other variables and functions that the outer function has access to). However, the outer function can’t get in (no access) to the variables and functions describe in detail (defined) inside the inner function. This gives a kind of encapsulation for the variables of the inner function. 

var pet = function(name) {   // The outer function defines a variable called "name"
  
  var getName = function() {
    
    return name;             // The inner function has access to the "name" variable of the 
    
    outer
                             //function
  
  }
  
  return getName;            // Return the inner function, thereby exposing it to outer 
  
  scopes

}

myPet = pet('Vivie');


myPet();                     // Returns "Vivie"

*(Mozilla and Individual Contributors, “Functions”, 2005-2021)*

### Using the Arguments Objects

Maintained in an array like object, are the arguments of a function. Inside a function, you have the ability to address the arguments passed to it as follows:

arguments[i]

Consider a function that contains several strings. The only correct argument for the function is a string that describes in detail the characters that keep apart  the items to concatenate. The function is defined as follows:

function myConcat(separator) {
   
   var result = ''; // initialize list
   
   var i;
   
   // iterate through arguments
   
   for (i = 1; i < arguments.length; i++) {
      
      result += arguments[i] + separator;
   
   }
   
   return result;

}

*(Mozilla and Individual Contributors, “Functions”, 2005-2021)*

### Arrow Functions

An Arrow Function Expression is a small in size (compact) other choice (alternative)  to a traditional function expression. However,  it's limited and can't be used in all situations. In comparison to Function Expressions, Arrow Functions have a shorter syntax. Arrow Functions are always unidentified. Below is an example of an Arrow Function.

var a = [
  
  'Hydrogen',
  
  'Helium',
  
  'Lithium',
  
  'Beryllium'

];

var a2 = a.map(function(s) { return s.length; });

console.log(a2); // logs [8, 6, 7, 9]

var a3 = a.map(s => s.length);

console.log(a3); // logs [8, 6, 7, 9]

*(Mozilla and Individual Contributors, “Functions”, 2005-2021)*

## Control Flow

The Control Flow is the sequence in which the computer does the job of  putting statements in a script. Unless your computer runs across conditionals and loops, which are very frequent structures that change the control flow, code will be run in order from the first line to the last line. In the example below, a script is used to validate user data from a web page. Validated data is being submitted from the script, however, if the user leaves a required field empty, the script prompts them to fill it in . To do this, the script makes use of  a conditional structure or if....else, so that different code executes depending on whether the form is complete or not.

if (field==empty) {
    
    promptUser();

} else {
    
    submitForm();

}

The above example may also be inside a function that runs whenever the user clicks the submit button for the form. The function also has the ability to include a loop, which says through all of the fields in the form, checking each one. So, as seen in the example, it's important to keep in mind that in Control Flow whenever you read a script, you must not only read from beginning to end, but also take a look at program structure and how it affects order of execution.

*(Mozilla and Individual contributors “Control Flow”, 2005-2021)*

## JavaScript Functions 

JavaScript Function is a block of code that is designed to perform a particular task. The task is done when something invokes (calls upon) it. When JavaScript Function is invoked, the code inside the function will do its task (execute). This will happen  

- When an event occurs (when a user clicks a button)

- When it is invoked (called) from JavaScript code

- Automatically (self invoked)

*(Refsnes Data, “JavaScript Functions”, 1999-2021)*

### JavaScript Function Syntax

A JavaScript Function is explained in great detail (defined) with the function keyword, which is proceeded by a name, and then followed by a parentheses ( ). The function names have the ability to contain letters, digits, underscores, and dollar signs (same rule as variables). The parentheses could possibly include parameter names separated by commas (parameter1, parameter2). The code to be put into place (executed) , by the function, is placed inside curly brackets { }. 

function name(parameter1, parameter2, parameter3) {
  
  // code to be executed

}

In the example above, the function parameters are enumerated within the parentheses in the function definition. Function arguments are the results taken in by the function when it is called upon (invoked). Within the function, the arguments (the parameters) act like local variables. 

*(Refsnes Data, “JavaScript Functions”, 1999-2021)*

### Function Return

A function will stop doing what it is supposed to do (execute), when JavaScript reaches a return statement. JavaScript will return to do what it is supposed to do (execute) with the code after the invoking statement, if the function was invoked from a statement. Functions will usually compute a return value, which is returned back to the caller. 

In the example below, is the calculation of the product of two numbers, and return the result:

let x = myFunction(4, 3);   // Function is called, return value will end up in x

function myFunction(a, b) {
  return a * b;             // Function returns the product of a and b
}

*(Refsnes Data, “JavaScript Functions”, 1999-2021)*

### Why Functions?

You are able to reuse code. You just have to define the code once, and then you are able to use it many time over, with different arguments, to produce different results. For example,

function toCelsius(fahrenheit) {
  
  return (5/9) * (fahrenheit-32);

}

document.getElementById("demo").innerHTML = toCelsius(77);

In the example above, toCelsius is referring to the function object, and toCelsius() refers to the function result. So, the () operator invokes the function. If you access a function without (), it will return the function object instead of the function result. 

*(Refsnes Data, “JavaScript Functions”, 1999-2021)*

### Local Variables

Variables that are declared within a JavaScript function, become local to the function. Local variables can only be reached from within the function. 

// code here can NOT use carName

function myFunction() {
  
  let carName = "Volvo";
  
  // code here CAN use carName

}

// code here can NOT use carName

*(Refsnes Data, “JavaScript Functions”, 1999-2021)*

## JavaScript Operators

The assignment operator (=) assigns a value to a variable.

let x = 7;         // assign the value 7 to x

let y = 4;         // assign the value 4 to y

let z = x + y;     // assign the value 11 to z (7+ 4)


*(Refsnes Data, “JavaScript Operators”, 1999-2021)*


The addition operator (+) adds numbers.

let x = 3;

let y = 9;

let z = x + y;

*(Refsnes Data, “JavaScript Operators”, 1999-2021)*


The multiplication operator (*) multiplies numbers.

let x = 3;

let y = 8;

let z = x * y;

*(Refsnes Data, “JavaScript Operators”, 1999-2021)*

### JavaScript Arithmetic Operators

+        Addition

-        Subtraction

*        Multiplication

**       Exponentiation 

/        Division

%        Modulus (Division Remainder)

++       Increment

--       Decrement

*(Refsnes Data, “JavaScript Functions”, 1999-2021)*


### JavaScript Assignment Operators

Operator	 Example	   Same As
=	          x = y	     x = y

+=	        x += y	   x = x + y

-=	        x -= y	   x = x - y

*=	        x *= y	   x = x * y

/=	        x /= y	   x = x / y

%=	        x %= y	   x = x % y

**=	        x **= y	   x = x ** y

*(Refsnes Data, “JavaScript Functions”, 1999-2021)*


### JavaScript String Operators

In JavaScript the plus sign (+) also has the ability to add (concatenate) strings. For example:

let text1 = “George”;
let text2 = “Smith”
let text3 = text1 + text2;

The result of text 3 will be:

George Smith
 
The plus and equal sign operator (+=) also have the ability to add (concatenate) strings;

let text1 = “That car “ ;
Text1 += “is very fast’’;

The result of text1 will be

That car is very fast.

### Adding Stings and Numbers

It’s important to point out, so that you’re able to distinguish that adding two numbers, will give you a sum; however, adding a number and a string will give you a string. For example:

let x = 7 + 8;
let y = “7” + 8;
let z = “Hello” + 7;

The result of x, y, and z will be:

15
78
Hello 7



### JavaScript Comparison Operators 

= =   equal to
= = =  equal value and equal type
! =  not equal
! = = not equal value or not equal type
>  greater than
<  less than
> = greater than or equal to
< = less than or equal to
?    ternary operator

 *(Refsnes Data, “JavaScript Operators”, 1999-2021)*


### JavaScript Logical Operators

&&  logical and
I I    logical or
!      logical not

*(Refsnes Data, “JavaScript Operators”, 1999-2021)*

###JavaScript Type Operators

typeof     Returns the type of a variable
instanceof  Returns true if an object is an instance of an object type  

*(Refsnes Data, “JavaScript Operators”, 1999-2021)*



[<==back](https://vonkrieg72.github.io/reading-notes/)