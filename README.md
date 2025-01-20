# Off-by-One Error in Java Array Iteration

This repository demonstrates a common off-by-one error in Java when iterating over an array.  The error arises from an incorrect loop condition that leads to accessing an index beyond the array's bounds, resulting in an `ArrayIndexOutOfBoundsException`.

## Bug Description

The `Bug.java` file contains a `for` loop that iterates from `0` to `arr.length` (inclusive).  This is incorrect because valid indices range from `0` to `arr.length - 1`.  Attempting to access `arr[arr.length]` results in an exception.

## Solution

The corrected code in `BugSolution.java` modifies the loop condition to iterate from `0` to `arr.length - 1`, effectively fixing the off-by-one error.