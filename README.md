# React useEffect Runs After Every Render

This repository demonstrates a common React performance issue related to the `useEffect` hook. The provided code shows an infinite loop in the console due to improper use of the `useEffect` hook.  The solution provides a corrected version that addresses the performance issue.

## Problem:

The original `MyComponent` uses `useEffect` without specifying dependencies.  This causes the effect to run after every render, leading to unnecessary re-renders and potential performance problems.  In this specific case, it creates an infinite loop of console logs.

## Solution:

The solution introduces an empty dependency array `[]` to the `useEffect` hook. This ensures the effect runs only once after the initial render, fixing the performance issue and preventing the console log infinite loop.
