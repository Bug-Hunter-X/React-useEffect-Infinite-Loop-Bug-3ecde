# React useEffect Infinite Loop Bug

This repository demonstrates a common React bug: an infinite loop caused by an incorrectly used `useEffect` hook.

The `bug.js` file contains the buggy code.  The `bugSolution.js` file provides the corrected version.  The issue stems from omitting the dependency array in `useEffect`, leading to the effect running after every render, triggering a new state update and restarting the cycle. This can significantly impact performance and cause application crashes.