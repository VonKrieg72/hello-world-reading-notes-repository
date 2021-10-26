# JS Debugging

## Error Handling and Debugging

In order to find out what’s causing errors in your JavaScript, it would be helpful to know how scripts are processed. In many cases it can be complex to know which order the statements are executed in, and some tasks aren’t able to be completed, until another statement or function has been run. **Execution Contexts** are the concept used by the JavaScript interpreter, and they correspond to the variable scope. There are three execution contexts: **global context, function context, and eval context,** and every statement within JavaScript will live in one of these three execution contexts. The global context refers to the code that is in the script, but not in the function, and there is only one global context per page. The function context refers to the code that is being run without a function, and each function has its own functional context. The eval contexts refers to when text is executed like code in an internal function called eval( ). The variable scope is made up of two scopes: **global scope and function level scope.** The global scope is where a variable is placed if you create one without using the keyword *var.* The variable also has global scope if it is declared outside of a function, because it can be used anywhere. Function level scope is where a variable is placed when it is declared within a function, because it can only be used within that function.  During the course of writing your code in JavaScript, whenever you come across an error, you will have to debug it, track down the source of it, and make the necessary changes to fix it. In many cases, debugging will involve deduction and eliminating the potential causes of what’s causing the error. You will want to narrow down the area, where problem is occurring, and:

-Look at the error message, and what it tells you.

-Check how far the script is running.

-Use breakpoints where things are going wrong. 

Once you have narrowed down the general area the problem is located at, then you can try to find the actual line of code that is the cause of the error.

-Once you have set breakpoints, you can see if the variables around them have the values you would expect them to. 

-Break down parts of the code, in order to test smaller pieces of the functionality.

-Check the number of parameters for a function or the number of items in an array. 

The JavaScript console is available on all modern web browsers and it is a valuable developer tool that tells you when there is a problem with a script, where to look for the problem, and what kind of issue it appears to be. JavaScript can display different types of error messages, and there will usually be seven different types of them on most browsers; however, there may be some varying error messages on others. For example, on the Google Chrome browser the seven different error objects are:

-SyntaxError

-ReferenceError

-EvalError

-URIError

-TypeError

-RangeError

-Error

-NaN (Not a Number)

If for any reason, you suspect that your code may fail, you can test it by using try, catch and finally statements. 

