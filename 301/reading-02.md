# Read: Class 02 - React Lifecycle & State Vs Props

## React Lifecycle
from: [React: Component Lifecycle Events](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)

1. Based off the diagram, what happens first, the `render` or the `componentDidMount`?
  - `render` happens first
2. What is the very first thing to happen in the lifecycle of React?
  - ##Mounting## is the first phase in the React lifecycle, Constructor, static, getDerivedStateFromProps, render, componentDidMount, and UNSAFE_componentWillMount occur in this order during mounting.
3. Put the following things in the order that they happen: `componentDidMount`, `render`, `constructor`, `componentWillUnmount`, `React Updates`.
  - `constructor`, `render`, `componentDidMount`, `React Updates`, `componentWillUnmount`
4. What does componentDidMount do?
  - It is where anything using a network request, or initializing the DOM should go. 

## React State Vs Props
from[React State Vs Props](https://www.youtube.com/watch?v=IYvD9oBCuJI)

1. What types of things can you pass in the props?
  - props can be thought of like parameters to a function
2. What is the big difference between props and state?
  - props you pass into a component. State is handled inside of a component and props are handled outside a component
3. When do we re-render our application?
  - when state is changed inside of your application, that section of the app gets re-rendered
4. What are some examples of things that we could store in state?
  - user input that should effect what is displayed on the page.
