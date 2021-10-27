# Read: 03 - Passing Functions as Props

## [React Docs-lists and keys](https://reactjs.org/docs/lists-and-keys.html)

1. What does .map() return?
  - .map() returns a new array
2. If I want to loop through an array and display each value in JSX, how do I do that in React?
  - you can use the .map() function to loop through the array.
  ```js
    //loops through the numbers array and  returns a new array with each element wrapped in <li> tags
    const numbers = [1, 2, 3, 4, 5];
    const listItems = numbers.map((number) =>
        <li>{number}</li>
    );
  ```
3. Each list item needs a unique key.
4. What is the purpose of a key?
  - Keys help React identify which items have changed, are added, or are removed. They give elements a stable identitly.

## [The Spread Operator](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)

1. What is the spread operator?
  - The spread operator is a quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function's arhuments (...)
2. List 4 things that the spread operator can do.
  1. Copy an array
  2. Concatenate or combine arrays
  3. Be used with Math functions
  4. Use an array as arguments
  5. Add an item to a list
  6. Add to state in React
  7. Combine objects
  8. Convert NodeList to an array
3. Give an example of using the spread operator to combine two arrays.
   ```js
    let nums = [1,2,3];
    let moreNums = [4,5,6];
    let allNums = [...nums,...moreNums];
   ```
4. Give an example of using the spread operator to add a new item to an array.
  ```js
    let nums = [1,2,3];
    let allNums = [...nums,4];
  ```
5. Give an example of using the spread operator to combine two objects into one.
  ```js
    let objOneName = {name: 'objOne'};
    let objOneData = {data: 'objOne data'};
    let objOne = {...objOneName,...objOneData};
  ```

## (How to Pass Functions Between Components)[https://www.youtube.com/watch?v=c05OL7XbwXU]

1. In the video, what is the first step that the developer does to pass functions between components?
  - they pass the method just like any other prop
2. In your own words, what does the `increment` function do?
  - the increment function uses the .map() method to loop through the people array to find objects with name values that equal the one passed through the function's parameter
3. How can you pass a method from a parent component into a child component?
  - You can pass methods through a components props
4. How does the child component invoke a method that was passed to it from a parent component?
  - the function is invoked through `this.props.functionName()`
