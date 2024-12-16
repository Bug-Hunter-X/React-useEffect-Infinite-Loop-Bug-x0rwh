# React useEffect Infinite Loop Bug

This repository demonstrates a common error in React's `useEffect` hook: an infinite loop caused by a missing dependency in the dependency array. 

## Description
The `useEffect` hook in `bug.js` attempts to log the current count, but without including `count` in its dependency array, the effect runs after every render, leading to an infinite loop of logging and re-renders.

## Solution
The `bugSolution.js` file shows the corrected version.  By adding `count` to the dependency array, the effect only runs when the `count` variable changes.