# Express.js Route Handler Missing Error Handling for Invalid User IDs

This repository demonstrates a common error in Express.js route handlers: missing error handling for invalid input.  Specifically, the code lacks proper handling for non-numeric user IDs.

## Bug

The `bug.js` file contains an Express.js route handler that retrieves a user based on their ID.  However, it fails to handle cases where the `userId` is not a valid integer.  This can lead to runtime errors or unexpected behavior.

## Solution

The `bugSolution.js` file provides a corrected version of the route handler. It includes robust error handling to check if `userId` is a valid integer and returns a 400 Bad Request error if it's not.