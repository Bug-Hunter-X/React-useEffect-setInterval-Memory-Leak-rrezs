# React useEffect setInterval Memory Leak

This repository demonstrates a common error in React applications involving the `useEffect` hook and `setInterval`.  The provided `MyComponent` uses `setInterval` to update a counter every second.  However, it omits the crucial cleanup function within `useEffect` to stop the interval when the component unmounts. This leads to a memory leak.

The solution shows how to properly implement cleanup to resolve this issue.