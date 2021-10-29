## [React Docs - Thinking in React](https://reactjs.org/docs/thinking-in-react.html)

1. What is the `single responsibility principle` and how does it apply to components?
    - a component should ideally only do one thing. If it grows, it should be broken down into smaller components
2. What does it mean to build a ‘static’ version of your application?
    - Building a non-interactive UI. The static version shouldn't use state at all
3. Once you have a static application, what do you need to add?
    - Next is to add the minimal representation of UI state. The key is to keep the DRY Principle in mind.
4. What are the three questions you can ask to determine if something is state?
    1. Is it passed in from a parent via props? If so, it probably isn't state.
    2. Does it remain unchanged over time? If so, it propbably isn't state.
    3. Can you compute it based on any other state or props in your component? If so, it isn't state.
5. How can you identify where state needs to live?
    1. Identify every component that renders something based on that state.
    2. Find a common owner component.
    3. Either the common owner or another component higher up in the hierarchy should own the state.
    4. If you can't find a component where it makes sense to own the state, create a new component soley for holding the state and add it somewhere in the hierarchy above hte common owner component.
## [Higher-Order Functions](https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK)

1. What is a “higher-order function”?
    - Functions that  operate on other functions by either taking them as arguments or returning them
2. Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?
    - returns a new arrow function that takes a parameter than compares it to the parameter passed to the containing funciton
3. Explain how either map or reduce operates, with regards to higher-order function
    - The map method transforms an array by applying a function to all of its elements and building a new array from the returned values.
