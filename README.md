# React Router v6 Catch-All Route Issue

This repository demonstrates a common issue encountered when using catch-all routes ('*') in React Router v6.  The problem is that the catch-all route fails to render when a non-matching path is entered, even though other routes are functioning correctly.

## Steps to Reproduce

1. Clone the repository.
2. Run `npm install` to install dependencies.
3. Run `npm start` to start the development server.
4. Navigate to a non-existent route (e.g., '/invalid-path').
5. Observe that the catch-all route does not render as expected.

## Solution

The solution involves ensuring the catch-all route is placed *after* all other routes.  This change is demonstrated in the `AppSolution.js` file.