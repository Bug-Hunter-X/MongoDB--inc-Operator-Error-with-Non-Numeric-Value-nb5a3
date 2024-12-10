# MongoDB $inc Operator Error with Non-Numeric Value

This repository demonstrates a common error when using the `$inc` operator in MongoDB update operations. The `$inc` operator is used to increment a numeric field by a specified value.  However, if a non-numeric value is provided, the operation will fail. 

The `bug.js` file contains the erroneous code, while `bugSolution.js` provides the correct implementation.

## Bug Description
The bug arises from attempting to increment the 'count' field with a string value ('abc').  MongoDB expects a numeric increment value.

## Solution
The corrected code ensures a numeric value is used with the `$inc` operator, resolving the error.