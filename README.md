# Append on Uninitialized Integer Variable in Go
This example demonstrates a common error in Go: attempting to use the `append` function on an uninitialized integer variable.

## Problem
The code snippet tries to append an integer to an integer variable, which is not a slice or array and not supported by Go's `append` function. Go compiler throws an error.

## Solution
The correct way is to declare the variable as a slice of integers, initialize it as an empty slice, and then use append.

## How to Reproduce
1. Save the code in `bug.go`
2. Run the code using `go run bug.go`
3. Observe the compile-time error.

## How to Fix
1. Refer to the fixed code in `bugSolution.go`
2. Run the code using `go run bugSolution.go`

The solution demonstrates the correct usage of the `append` function with slices.