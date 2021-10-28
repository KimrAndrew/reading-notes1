# Readings: React and Forms

## [React Docs - Forms](https://reactjs.org/docs/forms.html)
1. What is a 'Controlled Component'?
- A compnent that has its own state but uses the React state as a "single source of truth"
2. Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why?
- We should update the state as the user enters the response so the displayed value updates as they type
3. How do we target what the user is entering if we have an event handler on an input field?
- you can add a `name` attribute and let the handler function choose what to do based on the value of `event.target.name`

## [The Conditional (Ternary) Operator Explained](https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff)
1. Why would we use a ternary operator?
- it allows us to write more condensed if statements
2. Rewrite the following statement
```js
if (x===y) {
    console.log(true);
} else {
    console.log(false);
}
```

```js
x === y ? console.log(true) : console.log(false);
```
