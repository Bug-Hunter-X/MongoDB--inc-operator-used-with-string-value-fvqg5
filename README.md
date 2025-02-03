# MongoDB $inc Operator with String Value

This repository demonstrates a common error when using the `$inc` operator in MongoDB update queries. The `$inc` operator is designed to increment a numeric field by a specified value, but using a string value instead leads to unexpected results.

## Bug Description

The `$inc` operator in MongoDB is used to increment a numerical value in a document.  However, if you supply a string value to `$inc`, it will not increment the field as expected.

## Bug Solution

The solution involves ensuring that the value provided to the `$inc` operator is a number, not a string. This is achieved by modifying the update query to provide the correct numerical value.  See the `bugSolution.js` for a corrected example.

## How to Reproduce

1. Clone the repository.
2. Ensure you have MongoDB running.
3. Run `bug.js` and examine the output in the MongoDB shell.
4. Run `bugSolution.js` to see how it should be done.
