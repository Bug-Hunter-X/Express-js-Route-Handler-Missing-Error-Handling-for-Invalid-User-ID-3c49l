# Express.js Route Handler Missing Error Handling for Invalid User ID

This repository demonstrates a common error in Express.js route handlers: missing error handling for invalid input.  The example focuses on handling a missing or non-numeric user ID in a GET request.

## Bug

The `bug.js` file contains an Express.js route handler that retrieves a user by ID.  It attempts to parse the ID from the request parameters as an integer, but it fails to handle cases where the ID is not a number or is missing. This can lead to unexpected behavior or crashes.

## Solution

The `bugSolution.js` file provides a corrected version of the route handler. It includes error handling to check for invalid input and return appropriate error responses.