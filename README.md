# Dynamic Tailwind Classes Not Applying in Next.js

This repository demonstrates a common bug encountered when using Tailwind CSS with Next.js or similar frameworks. The issue arises when class names for styling are dynamically generated, and these generated names don't conform to Tailwind's rules. This results in styles not being applied correctly.

## Bug Description
When component props or state are used to build class names, incorrect formatting (typos, extra spaces, etc.) leads to Tailwind failing to recognize the classes.

## Bug Reproduction
1. Clone this repo.
2. Run `npm install`.
3. Run `npm run dev`.
4. Observe that the dynamically styled elements lack the expected Tailwind styling.

## Solution
The solution involves carefully checking the logic that generates class names. Ensure that no extra spaces or typos are present, and classes are properly concatenated.

## How to fix
Check the `bugSolution.js` file for the corrected code.  It includes thorough checks for class name validity to ensure correct formatting.