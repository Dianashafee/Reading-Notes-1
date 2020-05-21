# JS :

<br>

# ORDER OF EXECUTION :
To find the source of an error, it helps to know how scripts are processed, the order in which statements are executed can be complex; some tasks cannot complete until another statement or function has been run..

# EXECUTION CONTEXTS :
The JavaScript interpreter uses the concept of execution contexts, there is one global execution context; plus, each function creates a new execution context, they correspond to variable scope, and Every statement in a script lives in one of three execution contexts:
- GLOBAL CONTEXT
- FUNCTION CONTEXT
- EVAL CONTEXT (NOT SHOWN)

## What is stacks?
it happend when astatemnt needs data from another function, like tis kind of holder for each function..

![cap](https://3madov-77.github.io/Reading-Notes/Resorses/Capture10-1.PNG)

# EXECUTION CONTEXT & HOISTING :
Each time a script enters a new execution context, there are two phases of activity:
1. PREPARE
witch is often described as taking all of the variables and functions and hoisting them to the top of the execution context
2. EXECUTE

# ERRORS :
If a JavaScript statement generates an error, then it throws an exception(and that what error is), at that point, the interpreter stops and looks for exception-handling code

## ERROR OBJECTS :
Error objects can help you find where your mistakes are
and browsers have tools to help you read them, it will contain the following properties:

![cap](https://3madov-77.github.io/Reading-Notes/Resorses/Capture10-2.PNG)

There are seven types of built-in error objects in JavaScript witch is :

![cap](https://3madov-77.github.io/Reading-Notes/Resorses/Capture10-3.PNG)

## ERROR OBJECTS CONTINUED :
and it is:
- Syntax Error :the **SYNTAX IS NOT CORRECT**
- ReferenceError :**VARIABLE DOES NOT EXIST**
- EvalError :**INCORRECT USE OF `eval()` FUNCTION**
- URI Error :**INCORRECT USE OF URI FUNCTIONS**
- Type Error :**VALUE IS UNEXPECTED DATA TYPE**
- RangeError :**NUMBER OUTSIDE OF RANGE**
- Error :**GENERIC ERROR OBJECT**
- NaN :**NOT AN ERROR**

# HOW TO DEAL WITH ERRORS :
1: DEBUG THE SCRIPT TO FIX ERRORS
2: HANDLE ERRORS GRACEFULLY

# A DEBUGGING WORKFLOW :
## WHERE IS THE PROBLEM?
First, should try to can narrow down the area where the problem seems to be, and try:
1. Look at the error message
2. Check how far the script is running
3. Use breakpoints where things are going wrong

## WHAT EXACTLY IS THE PROBLEM?
1. When you have set breakpoints, you can see if the variables around them have the values you would expect them to. If not, look earlier in the script
2. Break down/break out parts of the code to test smaller pieces of the functionality
3. Check the number of parameters for a function, or the number of items in an array

> And be prepared to repeat the whole process if the above solved one error just to uncover another...

# BROWSER DEV TOOLS & JAVASCRIPT CONSOLE :
The JavaScript console will tell you when there is a problem with a script, where to look for the problem, and what kind of issue it seems to be


<br>
<br>
<hr>

**Always** you can contact me [Here](https://3madov-77.github.io/Side-Projects/Me/index.html)

<br>
<br>
<br>
<br>

[`Back To The Main Page`](https://3madov-77.github.io/Reading-Notes/)
