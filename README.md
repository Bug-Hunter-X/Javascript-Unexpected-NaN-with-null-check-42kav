# Javascript Unexpected NaN with null check
This repo contains a simple Javascript example that demonstrates unexpected NaN behavior when a function expects a null check but receives undefined. The bug occurs in the `foo` function, which attempts to handle null values correctly but fails to address undefined inputs.

## Bug Description
The function `foo` is designed to return 0 if the input `x` is null and `x + 1` otherwise. However, when `undefined` is passed as input, instead of an explicit error or default behavior, it returns `NaN`.

## Solution
The bug is addressed by adding an explicit check for `undefined` values using the strict equality operator (`===`). This ensures the function handles both `null` and `undefined` cases appropriately, producing expected results rather than `NaN`.  The solution provides robust error handling.