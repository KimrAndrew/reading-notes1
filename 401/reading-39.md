# React Context For Beginners

## What is React context?

- allows us to pass down and use data in whatever component we need in our React app without using props

## When should you React context

- data should not need to be updated often
- equivalent of global variables for React components

## What problems does React context solve?

- helps avoid prop drilling

## How do I use React context?

1. create context using `createContext`
2. wrap the context provider around your component tree
3. put any value on your context provider using value prop
4. Read that value within any component using the context consumer

## What is the useContext hook?

- instead of using render props, pass the entire context object to `React.useContext()`
