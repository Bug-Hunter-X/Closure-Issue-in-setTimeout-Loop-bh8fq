# JavaScript Closure Issue in setTimeout Loop

This repository demonstrates a common issue in JavaScript related to closures and the `setTimeout` function within loops.  The problem arises because the `setTimeout` callback function doesn't capture the value of `i` at the time it's scheduled, but rather captures the final value of `i` after the loop completes.  This results in unexpected behavior.

The `bug.js` file shows the problematic code, and the `bugSolution.js` file provides a solution using an immediately-invoked function expression (IIFE) to create a new scope for each iteration of the loop. 

This example highlights the importance of understanding JavaScript's closure mechanism when working with asynchronous operations.