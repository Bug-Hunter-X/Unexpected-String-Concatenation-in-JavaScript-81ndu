# JavaScript Type Coercion Bug

This repository demonstrates a common JavaScript bug caused by the language's loose typing system. Specifically, it showcases how the '+' operator can lead to unintended string concatenation rather than numerical addition. 

## The Bug

The `bug.js` file contains a function `foo` that is intended to add two numbers. However, if one of the inputs is a string, the '+' operator performs string concatenation instead of numerical addition. This can result in unexpected outputs and difficult-to-debug errors.

## The Solution

The `bugSolution.js` file demonstrates a simple solution: using the `Number()` function to explicitly convert the inputs to numbers before performing the addition. This ensures the '+' operator behaves as intended in all cases.

## How to Reproduce

1. Clone this repository.
2. Run `node bug.js` to see the unexpected string concatenation output.
3. Run `node bugSolution.js` to see the corrected output.