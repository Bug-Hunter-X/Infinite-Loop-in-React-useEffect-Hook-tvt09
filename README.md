# React useEffect Infinite Loop Bug

This repository demonstrates a common bug in React applications where an infinite loop is created by incorrectly using the `useEffect` hook.

## Bug Description

The `useEffect` hook is designed to perform side effects after a component renders.  However, if the state update within the `useEffect` hook depends on the state itself, and the state is not properly managed, this can lead to an infinite loop.

## Bug Reproduction

1. Clone this repository.
2. Run `npm install`.
3. Run `npm start`.
4. Observe the counter continuously incrementing, indicating the infinite loop.

## Bug Solution

The solution involves correctly managing the state update within the `useEffect` hook to prevent the infinite loop.

## Solution

The `bugSolution.js` file shows the corrected code, which uses `count` for the state update and prevents an infinite loop.