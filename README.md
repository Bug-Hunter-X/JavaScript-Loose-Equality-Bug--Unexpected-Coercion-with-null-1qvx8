# JavaScript Loose Equality Bug

This repository demonstrates a common error in JavaScript related to loose equality (`==`) and the handling of `null` values.

The `bug.js` file contains code with a subtle bug. The `bugSolution.js` file shows the corrected version, using strict equality (`===`) to avoid the problem.

## The Problem

JavaScript's loose equality (`==`) performs type coercion before comparison. This can lead to unexpected results, especially when comparing `null` with other values.

In the buggy code, `null` is loosely compared to 0.  This comparison evaluates to `true` because of type coercion, potentially leading to an incorrect program flow.

## The Solution

The solution is to use strict equality (`===`), which prevents type coercion. Strict equality checks both the value and the type of the operands, ensuring that comparisons are accurate.

## How to Run

1. Clone this repository.
2. Open `bug.js` and `bugSolution.js` in a JavaScript environment or web browser's console.
3. Run the functions and observe the different outputs.  The buggy function will potentially perform incorrect actions when either 'a' or 'b' are null. The solution will correctly handle the null values.