# JS DEBUGGING 

![](https://www.lambdatest.com/blog/wp-content/uploads/2018/07/534-x-300-5.jpg)

## ORDER OF EXECUTION

To find the source of an error, it helps to know how scripts are processed. The order in which statements are executed can be complex; some tasks cannot complete until another statement or function has been run.

## EXECUTION CONTEXTS

The JavaScript interpreter uses the concept of execution contexts. There is one global execution context; plus, each function creates a new new execution context. They correspond to variable scope.

Every statement in a script lives in one of three execution contexts:

> GLOBAL CONTEXT
> FUNCTION CONTEXT
> EVAL CONTEXT (NOT SHOWN)


# EXECUTION CONTEXT & HOISTING

Each time a script enters a new execution context, there are two phases of activity:

1. PREPARE

    * The new scope is created
    * Variables, functions, and arguments are created
    * The value of the this keyword is determined

2. EXECUTE

    * Now it can assign values to variables
    * Reference functions and run their code
    * Execute statements


## UNDERSTANDING SCOPE

In the interpreter, each execution context has its own va ri ables object. It holds the variables, functions, and parameters available within it. Each execution context can also access its parent’s variables object.

## UNDERSTANDING ERRORS

If a JavaScript statement generates an error, then it throws an exception. At that point, the interpreter stops and looks for exception-handl ing code.

## ERROR OBJECTS

Error objects can help you find where your mistakes are and browsers have tools to help you read them.

## HOW TO DEAL WITH ERRORS?

there are two things you can do with the errors:

1. DEBUG THE SCRIPT TO FIX ERRORS.
2. HANDLE ERRORS GRACEFULLY.


## DEBUGGING WORKFLOW

Debugging is about deduction: eliminating potential causes of an error. Here is a workflow for techniques you will meet over the next 20 pages. Try to narrow down where the problem might be, then look for clues.

## LOGGING DATA TO THE CONSOLE
The JavaScript console will tell you when there is a problem with a script, where to look for the problem, and what kind of issue it seems to be.