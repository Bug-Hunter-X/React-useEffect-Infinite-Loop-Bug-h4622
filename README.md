# React useEffect Infinite Loop

This repository demonstrates a common error in React's `useEffect` hook: creating an infinite loop by incorrectly updating state within the dependency array. The `bug.js` file contains the faulty code, while `bugSolution.js` provides the corrected version.

## Problem
The original code attempts to increment a counter in the `useEffect` hook, causing a continuous re-render. This is because the `count` variable is included in the dependency array, leading to an infinite loop. 

## Solution
The solution involves removing `count` from the dependency array or using a different approach such as `setTimeout` or `useRef` for side effects.