# Express.js Route Parameter Error Handling

This repository demonstrates a common error in Express.js route handlers: missing error handling for invalid input parameters.  Specifically, the example shows a route that fetches a user by ID, but fails to handle cases where the ID is not a valid number.

## Bug

The `bug.js` file contains the faulty code.  It attempts to parse the `userId` parameter as an integer without checking for potential errors (e.g., if the parameter is not a number or is missing). This can lead to crashes or unexpected behavior.

## Solution

The `bugSolution.js` file provides a corrected version of the code. It includes robust error handling to gracefully manage invalid user IDs and prevent application crashes.