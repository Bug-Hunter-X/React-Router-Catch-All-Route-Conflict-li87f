# React Router Catch-All Route Conflict

This repository demonstrates a common issue in React Router v6 where a catch-all route (`path="*"`) interferes with other routes, leading to incorrect component rendering or infinite redirect loops.

## Problem

The `path="*"` route, intended to handle any unmatched paths, can sometimes conflict with other routes in unexpected ways. This happens especially when routes are defined in a way that one might accidentally match paths that are intended to be handled by the catch-all route.  This is demonstrated in `bug.js`.

## Solution

The solution involves careful route ordering and potentially using more specific catch-all routes to avoid overlapping paths.  This is demonstrated in `bugSolution.js`.