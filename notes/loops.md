# Loops

Loops are an easy way to do actions repeatedly. There are several types of loops, but they essentially set to acheive the same goal.

There are two main groups of loops: `for` loops and `while` loops.

### For Loops

A `for` loop repeats until a specified condition evaluates to `false`.

A standard `for` loop looks like this:

```javascript
for ([initialExpression]; [conditionExpression]; [incrementExpression])
  statement
```
The flow of a `for` loop goes like this:

1. The initializing expression `initialExpression`, if any, is executed. This expression usually initializes one or more loop counters, but the syntax allows an expression of any degree of complexity. This expression can also declare variables. 
2. The `conditionExpression` expression is evaluated. If the value of `conditionExpression` is true, the loop statements execute. If the value of `condition` is false, the `for` loop terminates. (If the `condition` expression is omitted entirely, the condition is assumed to be true.)
3. The `statement` executes. To execute multiple statements, use a block statement (`{ ... }`) to group those statements.
4. If present, the update expression `incrementExpresion` is executed.
5. Control returns to Step 2.

Other types of `for` loops include:

- `for...in` loops
- `for...of` loops

In my experience, I tend to use `for...of` loops more often than `for...in` loops. Needing to loop over iterable objects (such as `Array`, `Map`, `Set`, `arguments`, etc.) occurs more often for me than needing to loop over object properties.

### While Loops

A `while` statement executes its statements as long as a specified condition evaluates to `true`. A `while` statement looks as follows:

```javascript
while (condition)
  statement
```
If the `condition` becomes `false`, statement within the loop stops executing and control passes to the statement following the loop.

The condition test occurs *before* `statement` in the loop is executed. If the condition returns `true`, `statement` is executed and the `condition` is tested again. If the condition returns `false`, execution stops, and control is passed to the statement following `while`.

To execute multiple statements, remember to use a block statement (`{ ... }`) to group those statements.
