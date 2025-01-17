# Unexpected Null Behavior with Strict Equality in JavaScript

This repository demonstrates a common, yet subtle, bug in JavaScript related to strict equality (`===`) and null checks. The issue arises when dealing with the potential for null values in arithmetic operations.

## The Problem

The provided `foo` function performs addition if both input parameters (`a` and `b`) are not null.  However, using strict equality (`===`) for null checks can lead to unexpected null results even if only one argument is null.

## The Solution

The solution involves being mindful of how null values interact with numerical operations. If you intend to treat null as zero in this context, then you need to explicitly handle type coercion before performing the addition.

## Running the Code

1. Clone this repository.
2. Navigate to the project directory in your terminal.
3. Open the files `bug.js` and `bugSolution.js` to see the buggy and corrected code respectively.
4. Run the JavaScript files using a Node.js interpreter: `node bug.js` and `node bugSolution.js`