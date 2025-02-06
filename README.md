# React 19 useEffect Dependency Bug
This repository demonstrates a common bug in React 19 applications involving the `useEffect` hook.  The bug arises from an incomplete dependency array, leading to unexpected behavior, specifically an infinite loop.

The `bug.js` file shows the incorrect implementation where the `count` state variable is not included in the dependency array of the `useEffect` hook. This omission causes the effect to run continuously, triggering an infinite loop that leads to performance issues and potential application crashes. 

The solution, shown in `bugSolution.js`, correctly includes 'count' in the dependency array resolving the issue. 

This example highlights the importance of carefully specifying dependencies in the `useEffect` hook to prevent such errors. 