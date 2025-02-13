# Unhandled Error in Async Express.js Request Handler

This repository demonstrates a common error in Express.js applications: unhandled errors within asynchronous request handlers.  The `bug.js` file shows an example where a simulated error is thrown inside a `setTimeout` callback, leading to a server crash without proper error handling.

The `bugSolution.js` file provides a solution by using a `try...catch` block to handle the potential error and send an appropriate error response to the client.  Proper error handling prevents unexpected server crashes and ensures more robust applications.

## How to Reproduce the Bug
1. Clone this repository.
2. Run `npm install` to install Express.js.
3. Run `node bug.js`.
4. Make a request to `http://localhost:3000/`.  The server will likely crash after a short delay because the error is unhandled.

## Solution
Refer to the `bugSolution.js` file for an implementation that demonstrates proper error handling.