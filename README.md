# Hack Recursive Function Bug

This repository demonstrates a common error in recursive functions written in Hack: Stack Overflow. The `foo` function calculates the factorial of a number. However, it lacks input validation and will cause a stack overflow if a negative integer is passed as an argument.

## Bug

The `bug.hack` file contains the buggy code. The factorial function is implemented recursively without handling negative inputs. When you try to run the `main` function with a large number or a negative number, you'll encounter a StackOverflowError.

## Solution

The `bugSolution.hack` file shows the solution: adding input validation to prevent the program from causing a stack overflow. The improved function now checks if the input is negative and throws an exception or returns a suitable value in such cases.