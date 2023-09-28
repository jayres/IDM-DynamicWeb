# Various JavaScript Notes from Class

** NOTE: IN PROGRESS **

## Conditional Statements in JavaScript

### if/else statement

The classic way to write a conditional statement. Note you may see me use a shortened syntax.

```js
const truthyValue = true;

if (truthyValue === true) {
  return "yup";
} else if (truthyValue === "true") {
  return "sort of";
} else {
  return "nope!";
}
```

### and (&&) + or (||) + ternary (val ? '' : '')

Inline ways to check if a value exists.

```js
const isTrue = true;
const isFalse = false;

const seeIfChainedValue = isTrue && "yup";

const seeIfOrValue = isTrue || isFalse;

const seeIfTernary = isTrue ? "yup" : "nope";
```

### Switch statements

A good way to simplify the conditional. This is useful when you want the expression inside switch statement to decide which case to execute. There is a matching pattern instead of a logical expression.

```js
const pet = "dog";

switch (pet) {
  case "dog":
    return "This is a dog";
  case "cat":
    return "This is a cat";
  default:
    return "no idea...";
}
```
