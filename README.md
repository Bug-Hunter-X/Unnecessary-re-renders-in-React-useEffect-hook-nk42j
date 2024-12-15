# Unnecessary Re-renders in React useEffect Hook

This repository demonstrates a common issue with the React `useEffect` hook: unnecessary re-renders due to missing or incorrect dependencies.

## Bug Description
The `useEffect` hook is designed to perform side effects after a component renders. However, if the dependency array is not properly specified, the effect will run after every render, which can lead to performance issues and unexpected behavior. In this example, the `useEffect` hook logs the current count to the console. However, because the dependency array is missing, the effect will run on every state update, leading to multiple log messages.