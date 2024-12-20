# Unexpected Re-renders in React useEffect Hook

This repository demonstrates a common issue with the React `useEffect` hook: unexpected re-renders due to missing dependencies in the dependency array.

## Bug

The `bug.js` file contains a component that uses `useEffect` to log the current count to the console. However, the dependency array is missing `count`, leading to infinite re-renders and potential performance issues. 

## Solution

The `bugSolution.js` file provides a corrected version of the component. By including `count` in the dependency array, the effect only runs when the `count` value actually changes. 