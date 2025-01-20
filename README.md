# Tcl Stack Overflow Bug

This repository demonstrates a common error in Tcl: a stack overflow caused by an improperly written recursive procedure.

The `bug.tcl` file contains the buggy code. The `bugSolution.tcl` file shows the corrected version.

## Bug Description

The `badproc` procedure attempts to calculate the factorial of a number using recursion.  However, it lacks a proper termination condition, causing infinite recursion. This leads to a stack overflow error when called with a non-zero argument.

## Solution

The `bugSolution.tcl` file demonstrates the correct implementation, introducing a proper base case to prevent infinite recursion and stack overflow errors.