# Unhandled Exception Crash in Node.js Server

This repository demonstrates a common error in Node.js applications: unhandled exceptions leading to server crashes.  The `bug.js` file showcases a server that crashes when a specific request is made due to a lack of proper error handling.  The `bugSolution.js` file provides a corrected version that demonstrates how to gracefully handle exceptions and prevent crashes.

## Bug

The `bug.js` server throws an uncaught exception when a request is made to `/error`.  This results in the server process terminating abruptly.

## Solution

The `bugSolution.js` file demonstrates proper error handling using a `try...catch` block to catch the exception and send a more appropriate response to the client, preventing the server from crashing.