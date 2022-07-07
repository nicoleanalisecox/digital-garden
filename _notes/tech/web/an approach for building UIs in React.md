---
title: an approach for building UIs in React
---

Summary of [Thinking in React](https://beta.reactjs.org/learn/thinking-in-react)

### Step 1: break UI into component hierarchy
- drawing boxes around components in mockup 
- think about any existing components that we are reusing
- thing about functionality/functions that the components will have
- arrange into a component hierarchy


### Step 2: build a static version 
- a static version just renders data, with no interactivity
- [[props]] only for this, no state as that's only for interactivity
- top-level component takes the data model as a prop


### Step 3: find the minimal but complete representation of UI state
> [[state]] is the minimal set of changing data that your app needs to remember 

- UI interactivity is basically letting users change the underlying data model 
- how can they do this? through state!
- think about the data you have, then determine which is state or which can be computed on demand. does it change over time? can it be computed from anything, e.g. something like reading the length of an array? 

### Step 4: give your state a home - identify where the state should live
- which component is responsible for changing the state/owning the state? 
- React uses one-way data flow

some steps to figuring this out:
1.  Identify _every_ component that renders something based on that state.
2.  Find their closest common parent component—a component above them all in the hierarchy.
3.  Decide where the state should live:
    1.  Often, you can put the state directly into their common parent.
    2.  You can also put the state into some component above their common parent.
    3.  If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common parent component.

### Step 5: reverse, reverse - add inverse data flow
- we have our app rendering with [[props]] and [[state]] flowing DOWN the hierarchy
- but we need to change the state depending on user input
- to do this we need to get the data flowing back up the other way, so the child components taking the input deeper in the hierarchy need to update the state in the parent at the top
- we can do this by passing in the state setter functions from the parent as props
- then we add and call the function that was passed down in the event handlers in the child component (onClick, onChange etc...)

Back to [[React]]