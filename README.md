# Node.js Server Error: listen EADDRINUSE

This repository demonstrates a common Node.js error: 'EADDRINUSE'. This error occurs when a server attempts to bind to a port that is already in use.

## Bug

The `bug.js` file contains a simple HTTP server that listens on port 8080. If you run this file and then try to run it again without stopping the first instance, you'll encounter the `EADDRINUSE` error.

## Solution

The `bugSolution.js` file provides a solution that gracefully handles the `EADDRINUSE` error. It attempts to bind to the port, and if it fails, it waits for a short period before trying again.