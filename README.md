# Julia Function Edge Case Bug

This repository demonstrates a subtle bug in a simple Julia function that arises when dealing with zero input. The function intends to square positive inputs and negate negative inputs. However, its handling of zero is implicit and could lead to unexpected behavior in different contexts.

## Bug Description
The `my_function` function does not explicitly define its behavior when the input `x` is zero. This can lead to issues depending on how the function is used or extended later.

## Solution
The solution clarifies the function's behavior for zero, ensuring predictable and consistent results. This is accomplished by adding an explicit `elseif` condition.