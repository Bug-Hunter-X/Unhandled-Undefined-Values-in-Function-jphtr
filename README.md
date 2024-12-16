# JavaScript Bug: Unhandled Undefined Values

This repository demonstrates a common JavaScript bug involving the improper handling of undefined values in a function.

## Bug Description

The `foo` function in `bug.js` correctly handles null values by returning null if either `a` or `b` is null. However, it does not handle undefined values. Passing undefined values to the function will result in a runtime error or unexpected behavior depending on how undefined is handled within the `+` operator.

## Bug Solution

The `bugSolution.js` file provides a solution by adding a check for undefined values using the strict equality operator (`===`).  This solution handles null and undefined values gracefully, returning null in either case.

## How to Reproduce

1. Clone the repository.
2. Open `bug.js` and observe the current implementation.
3. Run the script (e.g., using Node.js). Note that there are console.log() statements that show the different scenarios.
4. Examine `bugSolution.js` and notice the added check for undefined values.
5. Run `bugSolution.js` to observe the corrected handling of null and undefined values. 