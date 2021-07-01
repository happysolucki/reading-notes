# Programming with JavaScript

### Operators

The easiest way to understand operators in javascript is to relate them to how operators work in math. `= + - * /` are operators in math. They allow values to interact with each other. In javascript, there are both binary and unary operators as well as a special ternary operator that acts as a conditional.

This is an example of a binary operator:
```JavaScript

// Format
// operand1 operator operand2
3+4
2*5
14-7

```

A unary operator only requires a single operand, either before or after the operator:
```JavaScript

// operator operand
// operand operator
x++ // increments value of x by 1


```
There are various types of operators like:

- Assignment
- Comparison
- Arithmetic
- Bitwise
- Logical
- Conditional (ternary)

### Expressions

An *expression* is any valid unit of code that resolves to a value.

`3 + 4` is an expression. It uses the `+` operator to add three and four together without assigning the result, seven, to a variable.

Here are the following types of expressions:

- Arithmetic
- String
- Logical
- Primary expressions
- Left-hand-side expressions

Typically expressions contain an operator of some sort. The `this` and `new` keywords act as operators even though don't look like them.

#### this

Use the `this` *keyword* to refer to the current object. In general, `this` refers to the calling object in a method. Use `this` with the following notation:

```JavaScript
this['propertyName']
this.propertyName

```

#### new

You can use the `new` operator to create an instance of a user-defined object type or of one of the built-in objectt types.

```JavaScript
let objectName = new objectType([param1, param2, ..., paramN]);

```

### Functions

A function in JavaScript is similar to a procedure—a set of statements that performs a task or calculates a value, but for a procedure to qualify as a function, it should take some input and return an output where there is some obvious relationship between the input and the output. To use a function, you must define it somewhere in the scope from which you wish to call it.

Say you have a chunk of code but you want to use it again somewhere else in your code. Instead of just writing it out again, you can just wrap that piece of code in a function. Then whenever you need to recall that piece of code, you can just call the function instead. You could even pass that function into a different function.

#### Defining functions

Functions can be defined two different ways either through declaration or expression;

##### Function declarations

This is what a function declaration looks like:

```JavaScript

function square(number) {
  return number * number;
}

```

##### Function expression

This is what a function expression looks like:

```JavaScript

const square = function (number) {
  return number * number;
}

```
The example above is an anonymous function. You can provide a name to the function expression. Providing a name allows the function to refer to itself, and also makes it easier to identify the function in a debugger's stack traces:

```JavaScript

const square = function sqaureNum(number) {
  return number * number;
}

```
