# React Native useEffect Async State Update Error

This repository demonstrates a common error encountered when using the `useEffect` hook in React Native to update the component's state asynchronously.  The issue arises when the component unmounts before the asynchronous operation (like a network request) completes, resulting in an error similar to "Cannot update a component from its destructor".

The `bug.js` file showcases the problematic code that triggers this error. The `bugSolution.js` file provides a corrected implementation that uses a cleanup function and ensures state updates only occur when the component is still mounted.

## How to Reproduce

1. Clone this repository.
2. Navigate to the project directory.
3. Run `npm install` to install the necessary dependencies.
4. Run `npx react-native run-android` or `npx react-native run-ios` to run the app.

Observe the console for errors.  The solution file demonstrates how to prevent this error.