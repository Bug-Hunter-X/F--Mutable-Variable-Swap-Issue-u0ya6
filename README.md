# F# Mutable Variable Swap Issue

This example demonstrates a common pitfall when working with mutable variables in F#.  The `swap` function intends to exchange the values of `x` and `y`, but due to the way F# handles mutable variables within functions, it produces an unexpected result.

## Problem

The code uses mutable variables (`let mutable`) and attempts to swap their values using a temporary variable. However, the output is not what one might intuitively expect.