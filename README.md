# Incorrect useEffect Dependency Array

This repository demonstrates a common bug in React applications involving the `useEffect` hook and its dependency array.

## The Bug

The `bug.js` file contains a component that uses `useEffect` to update a counter every second. However, the dependency array is empty (`[]`), meaning the effect will only run once after the component mounts.  This means the counter never updates.

## The Solution

The `bugSolution.js` file demonstrates the correct usage of `useEffect`.  The `count` variable is included in the dependency array, ensuring that the effect re-runs whenever the `count` changes.