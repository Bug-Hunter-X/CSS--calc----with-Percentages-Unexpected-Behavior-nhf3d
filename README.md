# CSS calc() with Percentages Unexpected Behavior

This repository demonstrates an uncommon issue with the CSS `calc()` function when used with percentages.  The expected calculation does not produce the intended result.

## Bug Description

The `calc()` function is not correctly interpreting percentage values in certain contexts, leading to unexpected layout or styling problems.  This issue can be particularly tricky to debug because the syntax appears correct.

## Bug Reproduction

1. Clone this repository.
2. Open `bug.css` and `bugSolution.css`.
3. Examine the commented-out code in `bug.css` to see the issue.
4. Observe the corrected implementation in `bugSolution.css`.

## Solution

The solution involves a careful understanding of the order of operations within `calc()`. In the case of percentage values, the reference value (e.g., parent container width) is considered first before the percentage calculation happens.  Incorrect handling of this can result in unexpected behavior. The `bugSolution.css` provides the necessary correction.