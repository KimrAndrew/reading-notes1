# ES6 Syntax and Feature Overview

## Variable declaration

`let`
- block scope
- non hoisted
- can be reassigned

`const`
- block scope
- non hoisted
- can not be reassigned

## Arrow functions

Do not have their own `this`

cont func = (a,b) => {
    a + b
}

## Template literals

```
let word = 'Template'
sentance = `${word} literals allow you to embed expressions in strings.`
```

## Implicit returns

return keyword can be omitted if using arrow functions without a block body
```
let func = (a,b,c) => a + b + c
```

## Method definition shorthand

```
let obj = {
    a(c,d) {},
    b(e,f) {},
}
```

## Destructuring (object matching)

`let {a, b, c} = obj`

## Array iteration

```
for (let i of arr) {
    console.log(i)
}
```
