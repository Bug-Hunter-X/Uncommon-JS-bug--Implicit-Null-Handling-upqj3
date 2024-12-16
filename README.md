# Uncommon JavaScript Bug: Implicit Null Handling

This repository demonstrates a subtle JavaScript bug related to implicit null handling in function parameters.  Many developers might assume that JavaScript automatically handles null values, but this is not always the case.  The `bug.js` file showcases a function that fails if it receives null as input.  `bugSolution.js` provides the corrected version.

## How to Reproduce

1. Clone the repository.
2. Open `bug.js` and `bugSolution.js`.
3. Run the JavaScript code.

The `bug.js` version will show unexpected behavior when `null` is passed as an argument. The `bugSolution.js` file demonstrates the correct approach of explicitly handling null values.

## Bug Explanation

The main issue is that the addition operator (+) does not explicitly handle null values.  Attempting to add null to a number results in unexpected behavior. Explicitly checking for null using strict equality (`===`) prevents this problem.