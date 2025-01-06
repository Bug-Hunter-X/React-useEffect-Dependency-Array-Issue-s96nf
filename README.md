# React useEffect Dependency Array Issue

This repository demonstrates a common error in React's `useEffect` hook: forgetting to include state variables in the dependency array.  This can lead to infinite renders and unexpected behavior.

## Bug
The `bug.js` file contains a component with a `useEffect` hook that doesn't correctly list its dependencies.  This causes the effect to run on every render, creating an infinite loop.

## Solution
The `bugSolution.js` file shows the corrected component. By including `count` in the dependency array, the effect only runs when `count` changes.

## How to run
1. Clone the repo
2.  Run `npm install`
3.  Run `npm start`