# Unhandled Exception in Node.js HTTP Server

This repository demonstrates a common error in Node.js: unhandled exceptions in HTTP servers.  The `server.js` file contains code that throws an error without proper handling. This results in the server crashing. The solution in `server-solution.js` shows how to implement proper error handling to gracefully handle such exceptions.

## How to Reproduce

1. Clone the repository.
2. Run `node server.js`.
3. Observe the server crashing.
4. Run `node server-solution.js`.
5. Observe that the server handles the exception gracefully.

## Solution

The solution utilizes the `error` event listener on the HTTP server to catch exceptions and prevent crashes.  Logging the error is also good practice for debugging.