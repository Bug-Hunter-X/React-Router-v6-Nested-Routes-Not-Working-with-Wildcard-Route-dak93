# React Router v6 Nested Routes Issue

This repository demonstrates a common issue encountered when using nested routes with a wildcard route (*) in React Router v6.  The wildcard route unintentionally intercepts requests meant for nested routes, preventing them from rendering correctly.

## Problem

The provided `App.js` showcases this issue.  Despite defining nested routes, the wildcard route `/*` always renders, obscuring the nested routes.

## Solution

The `AppSolution.js` file offers a resolution by restructuring the routes to prioritize nested routes before the wildcard route. This ensures that nested routes are correctly matched and rendered before the catch-all wildcard route is used.