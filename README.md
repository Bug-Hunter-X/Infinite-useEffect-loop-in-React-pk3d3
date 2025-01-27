# React useEffect Infinite Loop Bug

This repository demonstrates a common React bug involving an infinite loop in the `useEffect` hook. The bug arises from an improperly configured dependency array, causing the effect to re-run endlessly after every render.

## Bug Description
The `useEffect` hook in the provided `MyComponent` function lacks a proper dependency array.  This causes the `console.log` statement to execute after every render, creating an infinite loop and impacting performance.  The solution involves correctly specifying the dependencies in the array.

## Solution
The solution is to include the `count` variable inside the dependency array of the useEffect hook to specify when it should re-run.  See `bugSolution.js` for the fix.