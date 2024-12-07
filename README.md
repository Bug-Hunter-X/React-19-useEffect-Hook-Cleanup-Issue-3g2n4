# React 19 useEffect Hook Cleanup Issue

This repository demonstrates a common error in React 19: forgetting to include a cleanup function in the `useEffect` hook when using `setInterval`.  This can lead to memory leaks and unexpected behavior.

## Bug
The `bug.js` file contains a component with an `useEffect` hook that uses `setInterval` to update a counter.  However, it's missing the cleanup function to stop the interval when the component unmounts.

## Solution
The `bugSolution.js` file provides the corrected version of the component, including the cleanup function using `clearInterval` to prevent memory leaks.