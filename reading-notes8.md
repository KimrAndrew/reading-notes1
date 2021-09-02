# LOOPS

## For Statements

- repeats until a specific condition is false

`for (\[initialExpression];\[conditionalExpression];\[incrementExpression]) {
    statement;
}`

`for(let i = 0; i < 5; i++) {
    console.log(i);
}`

output would be:
0
1
2
3
4

1. initialExpression is executed(i=0)
1. executes conditionalExpression(i<5)
1. if conditionalExpression is true: statement executes (console.log(i))
1. incrementExpression is executed (i++)
1. control returns to step 2

## While Statements

- executes as long as a specified condition is true

`while(condition){
    statement;
}`

- if the condition statement becomes false, the loop terminates and control moves on to the next statement
- make sure the condition statement will eventually become false or an infinite loop will result
