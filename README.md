# MongoDB $inc Operator Error with String Increment
This example demonstrates an error that occurs when using the `$inc` operator in a MongoDB update query with a string value instead of a number.  The `$inc` operator is designed to increment a numerical field by a specified amount. Using a string will cause the operation to fail or produce unexpected results.

## Bug Report
The original code attempts to increment the 'age' field by '1' (a string), which is incorrect.  This results in either an error or unintended behavior, depending on the MongoDB version and configuration.

## Solution
The solution involves ensuring that the value used with `$inc` is a number. The updated code uses the number 1, correctly incrementing the age field.
