# React Native State Access Error

This repository demonstrates a common error in React Native applications: attempting to access component state before the component has mounted or after it has unmounted. This often happens when working with asynchronous operations (like network requests) where data isn't immediately available.

## The Problem

The `bug.js` file shows a component that fetches data from an API.  It attempts to render data before it's available, leading to a runtime error.  This is a classic race condition between rendering and data fetching.

## The Solution

The `bugSolution.js` file presents a solution using conditional rendering. It checks if the data is loaded before attempting to render it.  This prevents errors by only rendering the UI once the data has been successfully fetched.

## How to run

1. Clone this repository.
2.  `cd` into the repository.
3. `npm install`
4. Run the project using your preferred React Native method (e.g., `npx react-native run-android` or `npx react-native run-ios`).

This example highlights the importance of careful state management and lifecycle handling in React Native development.