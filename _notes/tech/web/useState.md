---
title: useState
---

When you call useState, you are telling React that you want this component to remember something:

``` javascript
const [index, setIndex] = useState(0);
```

> 
> The convention is to name this pair like `const [something, setSomething]`. You could name it anything you like, but conventions make things easier to understand across projects.

-   Use a [[state]] variable when a component needs to “remember” some information between renders.
-   State variables are declared by calling the useState Hook.
-   The useState Hook returns a pair of values: the current state and the function to update it.
-   You can have more than one state variable. Internally, React matches them up by their order.
-   State is private to the component. If you render it in two places, each copy gets its own state.

[useState docs](https://beta.reactjs.org/apis/usestate)

Back to [[React]]