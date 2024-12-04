# Unhandled 'undefined' in Haskell

This repository demonstrates a common error in Haskell programming: the improper handling of the `undefined` value.  The `bug.hs` file contains code that uses `undefined` without proper error handling, resulting in a runtime exception.  The `bugSolution.hs` file provides a corrected version that gracefully handles potential undefined values.

## Problem

The `processMaybe` function uses `fromMaybe`, which throws an error if given an undefined value. The `main` function then calls `processMaybe` with `undefined`, leading to program termination.

## Solution

The solution involves checking for undefined values using pattern matching or other appropriate techniques before applying operations that might fail.  This prevents runtime crashes and produces more robust code. 