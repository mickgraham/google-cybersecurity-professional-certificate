# Module 1: Introduction to Python

## Overview

* Basics of programming
* Data types
* Variables
* Conditional statements
* Iterative statements

## Introduction to Python Programming in Cybersecurity

Security professionals use a variety of tools. One of those tools is computer programming. Python is considered to be a general-purpose language typically used to build websites and perform data analysis. In security, the main reason we use Python is to automate our tasks. Python is generally best for automating short, simple tasks such as:

* Searching through security logs for specific information.
* Periodically monitoring services like an access control list.
* Automated tasks like analysing network traffic.

There are several **advantages** Python has as a programming language:

* Python is user-friendly because it resembles human language, it requires less code, and it's easy to read.
* Python programmers also have the benefit of following standard guidelines to ensure consistency with the design and readability of code.
* Python also has an extensive collection of built-in code that we can import and use to perform many different tasks and there is a large amount of online support.
* Python can combine separate tasks into one workstream.

## Core Python Components

**Data types** classify data items in Python, much like categorising ingredients in cooking. Python uses several key data types, including string, float, integer, boolean, and **list**.

* **String**: An ordered sequence of characters (letters, symbols, spaces, numbers) enclosed in quotation marks, not used for calculations.
* Numeric (Float and Integer):
  * **Float**: Numbers with a decimal point (e.g., 2.1, 10.0).
  * **Integer**: Whole numbers without a decimal point (e.g., 0, -9, 5000).
* **Boolean**: Represents one of two values: True or False, primarily used for logic and comparisons.
* **List**: A collection of data items in a sequential form, enclosed in brackets, with individual items in quotation marks and separated by commas.

**Variables** inherit the data type of the object they store, and the **type()** function can be used to determine this. Variables are flexible; their stored data can be changed through reassignment, even to a different data type.

## Conditional Statements

**Conditional statements** enable automation by adding logic to code to allow specific actions to be executed based on whether certain conditions are met.

Conditional statements use the **if** keyword to evaluate a condition as **True** or **False**. If the condition is **True**, Python performs the indented action that follows the **if** statement. The **else** keyword allows for an alternative set of instructions to be executed if the preceding **if** condition (and any **elif** conditions) evaluates to **False**.

```
if status == 200:
    print("OK")
elif status == 400:
    print("Bad Request")
elif status == 500:
    print("Internal Server Error")
else:
    print("check other status")
```

## Iterative Statements

Iterative statements execute a set of instructions repeatedly, saving time and effort compared to typing the same code multiple times. There are two main types of loops: **for** loops and **while** loops:

**For** loops are used to iterate through a specified sequence, such as a list of usernames or characters in a string.
* The loop header defines the loop variable and the sequence to iterate through, ending with a colon, while the indented loop body contains the actions to perform in each iteration.
```
for i in range(5):
    print(i)
```

**While** loops iterate based on a condition, continuing as long as the condition remains True and exiting when it becomes False.
* Unlike for loops, the loop variable in a while loop is assigned outside the loop, and its value must be updated within the loop body to ensure the condition eventually becomes False.
```
i = 1
while i < 5:
    print(i)
    i = i + 1
```

The **break** keyword immediately exits a loop (either for or while) when a specified condition is met within an if statement.

The **continue** keyword skips the current iteration of a loop and proceeds to the next one when a specified condition is met.

## Glossary: Introduction to Python

Automation: The use of technology to reduce human and manual effort to perform common and repetitive tasks

Boolean data: Data that can only be one of two values: either True or False

Command-line interface: A text-based user interface that uses commands to interact with the computer

Comment: A note programmers make about the intention behind their code

Conditional statement: A statement that evaluates code to determine if it meets a specified set of conditions

Data type: A category for a particular type of data item

Dictionary data: Data that consists of one or more key-value pairs

Float data: Data consisting of a number with a decimal point

Integer data: Data consisting of a number that does not include a decimal point

Integrated development environment (IDE): A software application for writing code that provides editing assistance and error correction tools

Interpreter: A computer program that translates Python code into runnable instructions line by line

Iterative statement: Code that repeatedly executes a set of instructions

List data: Data structure that consists of a collection of data in sequential form

Loop variable: A variable that is used to control the iterations of a loop

Notebook: An online interface for writing, storing, and running code

Programming: A process that can be used to create a specific set of instructions for a computer to execute tasks

Set data: Data that consists of an unordered collection of unique values

String data: Data consisting of an ordered sequence of characters

Syntax: The rules that determine what is correctly structured in a computing language

Tuple data: Data structure that consists of a collection of data that cannot be changed

Type error: An error that results from using the wrong data type

Variable: A container that stores data
