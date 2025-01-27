# TypeScript Early Return Bug in Loop

This repository demonstrates an uncommon bug in TypeScript related to early returns within loops.  The bug is subtle and can be difficult to spot in larger codebases.

## Bug Description
The `printNumbers2` function intends to print numbers from 1 to n. However, due to the early return statement inside the loop, the function exits prematurely when `i` equals 3.  This behavior might not be immediately apparent, especially when dealing with more complex logic within the loop.

## How to Reproduce
1. Clone this repository.
2. Run `tsc bug.ts` to compile the code.
3. Run `node bug.js` to observe the output.

## Solution
The solution involves carefully considering the logic within the loop and ensuring that the early return doesn't cause unintended behavior.  In this case, removing the early return or adjusting the loop condition will fix the issue.

## Additional Notes
This bug highlights the importance of thoroughly testing code, particularly when using early returns or break statements within loops.  Type annotations don't always prevent unexpected behavior stemming from control flow issues.