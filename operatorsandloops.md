# Expressions and Operators

## Operators

The following types of operators exist in JavaScript

[Assignment operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators#assignment_operators) - Assignment operators give a value to its left operand which is dependent on the value of its right operand.

[Comparison operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators#comparison_operators) - Comparison operators make a comparison to its operands and give back a logical value, which is dependent on whether there is truth to the comparison. The operands have the possibility of being a numerical, string, logical, or object values.

[Arithmetic operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators#arithmetic_operators) - Arithmetic operators acquire values, which are numerical (either literals or variables) as their operands and give back a single numerical value. The standard arithmetic operators are addition (+), subtraction(-), multiplication (*), and division (/).

[Bitwise operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators#bitwise_operators) - A bitwise operator deal with and handle their operands as a set of 32 bits (zeros and ones), instead of decimals, hexadecimals, or octal numbers.

[Logical operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators#logical_operators) - Logical operators are usually utilized with Boolean (logical) values. In the event that they are, they give back a Boolean value.

[String operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators#string_operators) - Along with the comparison operators, which can be utilized on string values, the concatenation operator (+) concatenates two string values simultaneously, giving back another string that is the coming together of the two operand strings.

[Conditional (ternary) operator](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators#conditional_ternary_operator) - This is the only JavaScript operator that takes three operands. 

[Comma operator](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators#comma_operator) - This operator takes a look at both of its operands and gives back the value of the last operand. This operator is mostly utilized inside a for loop, in order to allow more than one variable to be updated each time through the loop

[Unary operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators#unary_operators) - This operator has only one operand

[Relational operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators#unary_operators) - This operator examines the quality of its operands and gives back a Boolean value, which is dependent on whether the comparison is true. 

*(Mozilla and individual contributors, “Expressions and operators”, 2005-2021)*

## Expressions

An expression is any logically correct unit of code that finds an answer to a value. Every syntactically correct expression finds an answer to some value; however, in concept, there are two types of expressions that have side effects. For example, those that administer values to a variable, and those that in some sense determine and therefore find an answer to a value.  In JavaScript there are the following expressional categories:

**-Arithmetic-** This determines the value to a number. For example 9.51413. Generally utilizes [Arithmetic operators]( https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators#arithmetic_operators)

**-String-** This determines the value to a character string. For example, “John” or “542”. Generally utilizes [String operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators#string_operators)

**-Logical-** This determines the value to true or false. This usually involves [Logical operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators#logical_operators) 

**-Primary expressions-** This is simple keywords and common expressions in JavaScrip.

**-Left hand side expression-** Left values are the end point of an assignment. 

*(Mozilla and individual contributors, “Expressions and operators”, 2005-2021)*

### Primary expressions

Primary expressions are general starting point keywords and common expression in JavaScript. For example, if you were to use the keyword **this** to regard  to a present object, basically most of the time, **this** refers to the calling object in a method.

*(Mozilla and individual contributors, “Expressions and operators”, 2005-2021)*

### Left Hand Side Expressions

Left values are the end purpose of an assignment.

You have the ability to  utilize the [new operator](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/new) to make an instance of a user identity determined object type or of one of the built in object types.

The [super keyword](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/super) is utilized to demand functions on an object’s parent. It is useful with [classes](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes) to demand the parent constructor.

*(Mozilla and individual contributors, “Expressions and operators”, 2005-2021)*


## Loops and iteration

Loops offer a fast and simple way to do something more than once. So, loops are essentially a computerized version of the game where you let someone know to take a certain amount of steps in one direction (call it X) and a certain amount of steps in another direction (call it Y). Many different types of loops exist, but they basically all do the same thing: they do an action again some number of times. 

*(Mozilla and individual contributors, “Loops and iteration”, 2005-2021)*

### for statement

A [for](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/for) loop over again and again until a specified condition determines to false. The JavaScript **for** loop has characteristics in common to the Java and C **for** loop. A for statement looks like:

for ([initialExpression] ; [conditionExpression] ; [incrementExpression]) 
statement

When a **for** loop does its job, the following happens:

- The **initialExpression** expression if any, is carried out, which most of the time initializes one or more loop counters, but the order of the language structure enables an expression of any level of complexity. 

- The **conditionalExpression** expression is determined. If the sum of the  conditionalExpression is true, the loop statements will do its job; however, if the sum of condition is false, the **for** loop terminates. 

- The statement does its job. To carry out and complete multiple statements, use a block statement {. . .} to put together those statements.

- If present, the update expression **incrementExpression** is carried out and completed

- Control will return to the 2nd step.

*(Mozilla and individual contributors, “Expressions and operators”, 2005-2021)*

### do. . .while statement

The **do. . .while** makes a statement over and over again until a specified condition determines to false. This is an example of a **do. . .while** statement

do
   statement
while (condition);

**statement** is always carried out once before the condition is looked at and verified. (In order to carry out and complete multiple statements, utilize a block statement ({ . . .}) to put together those statements.) 

If **condition** is **true,** the statement does its task again. At the conclusion of every task accomplished, the condition is verified. When the condition is **false,** the task in progress stops, and control travels to the statement following **do . . .while.**

In this example, the **do** loop iterates at least one time and continuously does so until **i** is no longer less than 5

let i = 0;
do {
    i += 1;
    console.log(i);
}   while  (i < 5) ;

*(Mozilla and individual contributors, “Expressions and operators”, 2005-2021)*

### while statement

A [while](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/while) statement carries out the task of its statements as long as a specified condition determines to **true.** A while statement looks like:

while (condition)
    statement


If the **condition** becomes **false**, **statement** inside the loop halts executing and control passes to the statement following the loop.

The condition test happens before **statement** in the loop is carried out. If the condition returns **true,** **statement** is carried out and the **condition** is tested again. If the condition gives you a  **false,** execution halts, and control is passed to the statement following **while.**

In order to execute multiple statements, utilize a block statement ( { . . . } ) to put together those statements.

In this example, the following **while** loop says as long as *n* is less than *3:*

let n = 1;
let x = 1;
while  (n < 3)  {
      n++;
      x  +=  n;
}

### labeled statement

A **label** gives you a statement along with an identifier that enables you to refer to it elsewhere through out your program. For example, you are able to use a label to identify a loop, and then utilize the **break** or **continue** statements to make it known whether a program should interrupt the loop or continue its execution.

The syntax of the labeled statement looks like:

label :
     statement

The sum (value) of **label** may be any JavaScript identifier that is not a reserved word. The **statement** that you identify with a label may be any statement. In the example below, the label **markLoop** identifies a **while** loop.

markLoop:
while  (theMark === true)  {
      doSomething( );
}

### break statement

The **break** statement can be utilized to terminate a loop, **switch** or in conjunction with a labeled statement.

In the event that you utilize **break** without a label, it terminates the innermost enclosing **while,** **do-while,** **for,** or **switch** immediately and transfers control to the following statement. In the event that you utilize **break** with a label; it terminates the specified labeled statement. The ordered language (syntax) of the **break** statement looks like the following:

break;
break  [ label ] ;

The first form of the ordered language (syntax) terminates the innermost enclosing loop or **switch.** The second form of the ordered language terminates the specified enclosing labeled statement. In the following example, it says that through the elements in an array until it locates the index of an element whose value is **theValue:**

for  ( let i = 0;  i < a. length ;  i ++ )  {
   if   (a [ i ]  = = = theValue )   {
        break;
     }
}

*(Mozilla and individual contributors, “Expressions and operators”, 2005-2021)*

### continue statement

The **continue** statement can be utilized to restart a **while,** **do-while,** **for,** or **label** statement. 

Whenever you utilize **continue** without a label, it does away with (terminates) the current iteration of the innermost enclosing **while,** **do-while,** of **for** statement and keeps doing the execution of the loop along with the next iteration. In contrast to the break statement, **continue** does not do away with (terminate) the execution of the loop completely. In a **while** loop, it goes back to the condition. In a **for** loop, it jumps to the **increment-expression.** Whenever you utilize **continue** along with a label, it applies to the looping statement identified along with that label. The ordered language (syntax) of the **continue** statement looks like:

continue  [ label ] ;

*(Mozilla and individual contributors, “Expressions and operators”, 2005-2021)*

### for . . . in statement

The **for . . . in** statement declares a specified variable over all the listed properties of an object. For each distinct property, JavaScript completes the task of the specified statements. A **for . . . in** statement looks like :

for  ( variable  in  object )
   statement

*(Mozilla and individual contributors, “Expressions and operators”, 2005-2021)*

### for . . . of statement

The **for . . . of** statement makes a loop declaring over **iterable objects** (including **Array,** **map,** **set,** **arguments** object and so on), calling upon a custom iteration hook with statements to be completed for the value of each distinct property.

for  (variable  of object)
   statement

*(Mozilla and individual contributors, “Expressions and operators”, 2005-2021)*


 
 [<==back](README.md)