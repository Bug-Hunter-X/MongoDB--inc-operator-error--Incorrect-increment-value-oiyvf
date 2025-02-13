# MongoDB $inc Operator Error
This repository demonstrates a common error when using the `$inc` operator in MongoDB update operations.

The error occurs when using an incorrect data type for the increment value. The `$inc` operator expects a number, but using a string instead results in an unexpected behavior or an error.

## Bug
The `bug.js` file contains code that attempts to increment the 'age' field in a MongoDB document using a string value for the increment. This leads to an error because the $inc operator expects a numeric value.  The error message will indicate an invalid operator usage.

## Solution
The `bugSolution.js` file provides the corrected code, where the increment value is a number, correctly updating the document.

## How to reproduce
1. Clone this repository.
2. Ensure you have a MongoDB instance running.
3. Run `bug.js` (you'll get an error). 
4. Run `bugSolution.js` (this should work correctly).
