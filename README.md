# F# Mutable Variable Bug

This repository demonstrates a common error in F# involving mutable variables and function calls. The `addOne` function calculates `x + 1`, but it doesn't modify the original mutable variable `x`.  The code intends to demonstrate the change to `x`, but due to immutability within functional programming concepts, it fails to reflect the expected behaviour.

## Bug
The `bug.fs` file contains the erroneous code.  It shows that while the function correctly adds one, the original variable remains unchanged leading to unexpected output.

## Solution
The `bugSolution.fs` file provides a corrected version.  This version demonstrates that if you intend to change the value of a mutable variable within a function, it must be explicitly modified within the function itself.