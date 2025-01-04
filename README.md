# Off-by-One Error in C++ Vector Iteration

This repository demonstrates a common off-by-one error in C++ when iterating over a vector using a for loop.

The bug occurs in the `main` function where the loop condition `i <= vec.size()` attempts to access an element beyond the valid range of the vector, leading to undefined behavior.

The solution corrects the loop condition to `i < vec.size()`, ensuring that the loop iterates through all valid elements.

## How to reproduce the bug

1. Compile and run `bug.cpp`.
2. Observe the out-of-bounds access and potential crash or unexpected behavior.

## How to fix the bug

1. Replace `i <= vec.size()` with `i < vec.size()` in the for loop condition in `bugSolution.cpp`.
2. Compile and run `bugSolution.cpp` to see the correct output.
