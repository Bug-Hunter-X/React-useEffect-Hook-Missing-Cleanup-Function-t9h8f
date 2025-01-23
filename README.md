# React useEffect Hook Missing Cleanup Function

This repository demonstrates a common error in React applications: forgetting to include a cleanup function in the `useEffect` hook.  This can lead to memory leaks and unexpected behavior.

## The Problem

The `bug.js` file contains a component that updates the document title whenever the count changes. However, it's missing the return statement which is crucial for the cleanup function. Without this, the component continuously updates the document title even after it's unmounted, leading to potential issues.

## The Solution

The `bugSolution.js` file shows the corrected code. The `useEffect` hook now includes a return statement that removes the event listener, preventing memory leaks and ensuring proper cleanup when the component unmounts.

## How to Run

1. Clone this repository.
2. Navigate to the project directory.
3. Run `npm install` to install dependencies.
4. Run `npm start` to start the development server. 

Observe the console and browser behavior to understand the difference.