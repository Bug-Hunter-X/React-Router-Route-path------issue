# React Router Catch-All Route Issue

This repository demonstrates a common issue with React Router's catch-all route (`path="/*"`). The catch-all route unexpectedly matches all paths, preventing other routes from working correctly.

## Problem

The provided `App.js` contains three routes: one for the home page, one for an about page, and a catch-all route for handling 404 errors. The expectation is that the catch-all route only matches when no other routes match.  However, the catch-all route is always selected regardless of the URL.

## Solution

The solution, provided in `AppSolution.js`, addresses this by ensuring the catch-all route is placed last in the `Routes` component. This ensures that more specific routes are matched first, before falling back to the catch-all.
