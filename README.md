# Julia Function Bug: Incorrect Result for Negative Input

This repository demonstrates a subtle bug in a Julia function that produces an incorrect result when given a negative input. The issue stems from the way Julia handles operator precedence and the unintended order of operations.

The `bug.jl` file contains the buggy function and an example of its unexpected behavior. The `bugSolution.jl` file provides a corrected version of the function that addresses the precedence issue.

## Bug Description

The function `my_function` is intended to return the square of its input if the input is positive, and the negative of the square if the input is negative. However, due to the order of operations, it does not correctly compute the negative square for negative inputs.

## Solution

The corrected version of the function uses explicit parentheses to enforce the correct order of operations.