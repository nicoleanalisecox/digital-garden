---
title: React
---

## How React Works
### Components
What React is made up of. Components are [[JavaScript]] functions that return [[JSX]] markup.

### Things we can do  in React

**Conditional rendering**: You can conditionally display React components with if / else, conditional operators or the logical && syntax.  

**Rendering lists**: we can use for loops and .map() to render lists. Each item in a list needs a unique key attribute so it can tell what's affected if we insert, delete or reorder items. 

**Respond to events**: _Event handler_ functions can be declared inside components to respond to events. We pass event handlers down (not call them), then React calls the function when the event happens (e.g. on button click).

```JavaScript
function MyButton() {
  function handleClick() {
    alert('You clicked me!');
  }

  return (
    <button onClick={handleClick}>
      Click me
    </button>
  );
}

```

### Data in React
These are partners in crime and work together. For example, parent components usually keep information in state but then also pass it down to their children through props. 
[[props]]
[[state]]

React Life Cycle

### React Hooks
Hooks let you 'hook into' a component's [[render cycle]]. They are special functions are are only available while react is rendering. They can only be called at the top level of your components.
- [[useState]]
- [[useEffect]]
- useRef
- useCallback
- useMemo
- useReducer
- useContext

### Practices & Patterns
[[an approach for building UIs in React]]
[[managing state in React]]
