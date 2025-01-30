# React Native useEffect Cleanup Function Error

This repository demonstrates a common but often elusive bug in React Native applications involving the `useEffect` hook and its cleanup function.  The bug arises when the cleanup function attempts to interact with component state or props after the component has unmounted.  This typically happens during asynchronous operations, making debugging more challenging.

The `useEffectBug.js` file showcases the problematic code. The `useEffectSolution.js` file demonstrates a corrected version with proper error handling to prevent crashes and ensure smooth application operation.

## Reproduction Steps

1. Clone this repository.
2. Navigate to the directory.
3. Run `npm install` to install dependencies.
4. Run `npx react-native run-android` (or `npx react-native run-ios`) to run the application.
5. Observe the error message in the console (in `useEffectBug.js`) or the successful execution in (`useEffectSolution.js`).