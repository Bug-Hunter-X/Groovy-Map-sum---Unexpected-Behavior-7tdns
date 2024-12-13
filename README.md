# Groovy Map sum() Unexpected Behavior

This repository demonstrates a common, yet subtle, error in Groovy when using the `sum()` method with Maps.  The `sum()` method is designed to work with collections of numbers (like Lists), not Maps.  Attempting to call `sum()` on a Groovy map will lead to a `MissingMethodException`.

The `bug.groovy` file shows the error in action.  The solution, demonstrated in `bugSolution.groovy`, involves using the `values()` method to extract the numerical values from the map before summing them.

## How to reproduce

1. Clone this repository.
2. Open `bug.groovy` in a Groovy environment.
3. Run the script. Observe the `MissingMethodException`.
4. Open `bugSolution.groovy`. Run it to see the corrected behavior. 

This example highlights the importance of understanding the intended use of Groovy's built-in methods. Always be mindful of the data type you're working with, and consult the Groovy documentation when necessary.