---
title: state
---

State is how React components can 'remember' things at a point in time, so it can keep track of some information and change it in response to certain interactions that happens. 

### Why can't I use a regular ol' variable for this? 
1.  **Local variables don’t persist between renders.** When React renders this component a second time, it renders it from scratch—it doesn’t consider any changes to the local variables.
2.  **Changes to local variables won’t trigger renders.** React doesn’t realize it needs to render the component again with the new data.

### What needs to happen to update a component with fresh data?
To update a component with new data, two things need to happen:
1.  **Retain** the data between renders.
2.  **Trigger** React to render the component with new data (re-rendering).

### [[useState]] to the rescue! What powers does it give us?
1.  A **state variable** to retain the data between renders.
2.  A **state setter function** to update the variable and trigger React to render the component again.


[State: a component's memory](https://beta.reactjs.org/learn/state-a-components-memory)

Back to [[React]]