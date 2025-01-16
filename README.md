# Unexpected Behavior of Mutable Variable Swapping in F#

This repository demonstrates a common error in F# related to the unexpected behavior of mutable variable swapping.  F#'s pass-by-reference nature for mutable variables can lead to surprising outcomes when attempting to swap values.

The `bug.fs` file shows an example of a seemingly correct swap function that doesn't produce the intended result.  The `bugSolution.fs` demonstrates a corrected version using tuples to avoid unexpected mutations.

## Bug Description:

When attempting to swap the values of two mutable variables using a function in F#, the original variables are modified directly due to pass-by-reference. This often results in unintended consequences, and the code doesn't behave as expected.