# Unhandled Promise Rejection in Express.js Application

This repository demonstrates a common error in Node.js applications using Express.js: unhandled promise rejections.  The provided code simulates an asynchronous operation that might fail.  The application fails to handle the rejection properly, leading to crashes or unexpected behavior.

## Bug Description

The `someAsyncOperation` function simulates an asynchronous operation that randomly fails.  If the operation fails, the error is logged to the console but not handled gracefully.  This can lead to the application crashing or behaving erratically.

## Solution

The solution involves using a `try...catch` block or proper error handling within the asynchronous operation to prevent unhandled promise rejections.  The provided `bugSolution.js` demonstrates the correct approach.

## How to reproduce

1. Clone the repository.
2. Run `npm install express`.
3. Run `node bug.js`.
4. Observe that the application might fail randomly and the console will display error messages.
5. Run `node bugSolution.js` to see the corrected implementation.