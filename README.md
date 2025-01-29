# JavaScript Type Coercion Bug

This repository demonstrates a common, yet subtle, bug in JavaScript related to type coercion when using the + operator.  The bug showcases how JavaScript's loose typing can lead to unexpected results, specifically when mixing strings and numbers.

## Bug Description
The `bar` function uses `foo` to add two numbers, then doubles the result. However, if a string is passed as an argument, the addition (`+`) operator performs string concatenation instead of numeric addition. This leads to `NaN` (Not a Number) when the result is multiplied by 2.

## Bug Solution
The solution involves explicit type checking or conversion to ensure that numeric operations are performed with numbers.