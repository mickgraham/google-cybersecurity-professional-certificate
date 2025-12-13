# Module 2: Write effective Python code

## Overview

* Functions
* Modules and libraries
* Code readability

## Introduction to Functions

**Functions** are reusable sections of code that automate repetitive tasks within a program. They improve efficiency by performing repetitive activities and can be called multiple times from anywhere in a program, reducing the need to write the same code repeatedly.

* **Built-in** functions are functions that exist within Python and can be called directly. The `print()` function is an example of a built-in function.
* **User-defined** functions are functions that programmers design for their specific needs. To define a function, you need to include a function header and the body of your function.

## Arguments, Parameters, and Return Statements

* **Parameters** are placeholders defined in a function's definition, allowing it to accept external information.
* **Arguments** are the actual data passed into a function when it is called, corresponding to its parameters.
* A **return** statement executes inside a function and sends information back to where the function was called.

When calling a function that expects parameters, provide the arguments in the same order as the parameters are defined. Arguments can be specific values or variables, and they are also separated by commas when multiple are used.

In the following example, the information returned from the call to **remaining_login_attempts** is stored in a variable called **remaining_attempts**. Then, this variable is used in a conditional that prints a **"Your account is locked"** message when **remaining_attempts** is less than or equal to 0.

```
def remaining_login_attempts(maximum_attempts, total_attempts):
    return maximum_attempts - total_attempts
remaining_attempts = remaining_login_attempts(3, 3)
if remaining_attempts <= 0:
    print("Your account is locked")
```

**Global variables** are defined outside of functions and are accessible throughout the entire program.

**Local variables** are assigned within a function (including parameters) and can only be accessed inside that function. It's best practice to avoid reusing global variable names as local variables to prevent confusion.

## Code Readability

Python's readability is enhanced by community-shared guidelines called style guides, which promote clean and neat code.

**PEP 8**, a **Python Enhancement Proposal**, offers stylistic suggestions for Python programmers, aiming for consistency and easier code comprehension.

* **Comments** are notes within code that explain the programmer's intent, indicating what the code does and why.
  * PEP 8 recommends clear, up-to-date comments to help others understand the code's context and purpose.
The Role of Indentation in Readability and Execution
* **Indentation**, the space at the beginning of a line of code, improves readability and ensures correct code execution.
  * Proper indentation groups related lines of code, establishing connections and dictating execution flow, as seen in conditional statements.

## Learn from the Python Community

* A **library** is a collection of modules that offer reusable code for various functionalities.
* A **module** is a Python file containing functions, variables, and classes, acting as a saved collection of useful code.

The **Python Standard Library** is a comprehensive set of pre-installed modules that come with Python. Examples include the `re` module for searching patterns in log files and the `csv` module for working with CSV files.

**External Libraries** extend Python's capabilities. Examples include `Beautiful Soup` for parsing HTML and `NumPy` for numerical computations, both useful for cybersecurity tasks like network traffic analysis.

To import these modules from the Python Standard Library, you must use the **import** keyword. Syntax varies depending on whether or not you want to import the entire module or just specific functions from it. External libraries can also be imported into Python, but they need to be installed first.

## Glossary: Write effective Python code

Argument (Python): The data brought into a function when it is called

Built-in function: A function that exists within Python and can be called directly

Comment: A note programmers make about the intention behind their code

Function: A section of code that can be reused in a program

Global variable: A variable that is available through the entire program

Indentation: Space added at the beginning of a line of code

Library: A collection of modules that provide code users can access in their programs

Local variable: A variable assigned within a function

Module: A Python file that contains additional functions, variables, classes, and any kind of runnable code

Parameter (Python): An object that is included in a function definition for use in that function

PEP 8 style guide: A resource that provides stylistic guidelines for programmers working in Python

Python Standard Library: An extensive collection of Python code that often comes packaged with Python

Return statement: A Python statement that executes inside a function and sends information back to the function call

Style guide: A manual that informs the writing, formatting, and design of documents

User-defined function: A function that programmers design for their specific needs