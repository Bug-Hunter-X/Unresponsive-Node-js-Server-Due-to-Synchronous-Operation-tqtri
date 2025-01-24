# Unresponsive Node.js Server

This repository demonstrates a common issue in Node.js where a long-running synchronous operation in a request handler blocks the event loop, making the server unresponsive.  The `bug.js` file contains the problematic code.  The solution, found in `bugSolution.js`, illustrates how to use asynchronous operations or worker threads to avoid this issue. 

## How to reproduce
1. Clone this repository.
2. Run `node bug.js`.
3. Try to access `http://localhost:3000` in your browser. You'll notice significant delays or unresponsiveness.  The server might appear to hang.

## Solution
Refer to `bugSolution.js` for a corrected version that uses asynchronous operations.