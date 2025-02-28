# Tailwind Dark Mode Issue

## Problem Description

This repository demonstrates an issue with Tailwind CSS dark mode where applying dark mode classes to one element unexpectedly affects other elements.

### Issue Details

1. **Dark Mode Not Working Correctly**: The dark mode toggle functionality is not properly applying dark mode styles as expected.

2. **CSS Class Leakage**: When applying a dark mode class like `dark:text-red-400` to a button, the style unexpectedly affects other elements on the page that shouldn't inherit this styling.

## Reproduction Steps

1. Toggle dark mode on the page
2. Observe that elements with specific dark mode classes affect unrelated elements
3. For example, a button with `dark:text-red-400` causes text color changes in other components

## Environment

- Tailwind CSS version: 4.0.9
- Operating System: Windows

