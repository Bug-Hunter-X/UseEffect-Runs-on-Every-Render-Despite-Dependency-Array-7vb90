# React useEffect Runs on Every Render Bug

This repository demonstrates a common React bug where the `useEffect` hook runs on every render, even when a dependency array is provided.  The issue stems from an improper usage of the functional update pattern within the `setCount` function. 

The `bug.js` file shows the problematic code. The `bugSolution.js` file provides the corrected version.

## Bug Description
The `useEffect` hook, intended to run only when its dependencies change, is running on each render. This causes performance issues and unexpected behavior. The incorrect `setCount` implementation does not guarantee updating the state with the correct value.