# React Router Dom Catch-All Route Issue

This repository demonstrates a common issue encountered when using the catch-all route `/*` in `react-router-dom`. The problem arises because the catch-all route matches all paths, overriding other, more specific routes.

## The Problem

The provided `App.js` demonstrates an implementation where a catch-all route (`/*`) is used with other defined routes. Despite having specific routes like `/` and `/about`, any navigation will lead to the NotFound component due to the catch-all route's behavior.

## The Solution

The solution, in `AppSolution.js`, shows how to correctly use the catch-all route by placing it as the *last* route in the `Routes` component. This ensures that it only matches paths that don't match any other route.