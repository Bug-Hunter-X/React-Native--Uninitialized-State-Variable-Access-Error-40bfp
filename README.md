# React Native: Uninitialized State Variable Access Error

This repository demonstrates a common error in React Native: accessing a state variable before it has been initialized.  The error occurs because the state variable is accessed in the render method before the component has mounted and the state has been set.

## Problem

The `bug.js` file contains a component that attempts to access `this.state.count` within the `render` method before the component has finished mounting. This results in the error: "Cannot read properties of undefined (reading 'count')".

## Solution

The `bugSolution.js` file provides a solution to this problem by using conditional rendering to only render the `Text` component once the state has been initialized. Alternatively, providing a default value for state or using functional component state can also solve this problem. 