# Typescript Labs

## Lab 17: Typing Functions

file: `/src/17-function-types.problem.ts`

Now we'll move on to typing functions.

We have an `addListener` function here:

```ts
const addListener = (onFocusChange: unknown) => {
  window.addEventListener("focus", () => {
    onFocusChange(true);
  });

  window.addEventListener("blur", () => {
    onFocusChange(false);
  });
};

```

The type of `onFocusChange` that is passed in is currently unknown.

What we want it to be is a function that will take in a single boolean argument.

Challenge
Your challenge is to visit the TypeScript Docs and work out how to appropriately type the `onFocusChange` function.

