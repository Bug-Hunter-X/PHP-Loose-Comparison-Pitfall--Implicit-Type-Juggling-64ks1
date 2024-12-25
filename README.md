# PHP Loose Comparison Pitfall

This repository demonstrates a common error in PHP related to loose comparison (==) and implicit type juggling.  Loose comparison can lead to unexpected results when comparing variables of different types.  The example showcases how a string '10' can be considered equal to an integer 10 due to PHP's automatic type conversion.

## Bug

The `bug.php` file contains code that uses a loose comparison, which can lead to unexpected behavior if strict type checking is required. The code compares a string '10' to an integer 10, resulting in true condition. 

## Solution

The `bugSolution.php` file provides a corrected version using strict comparison (===) to prevent implicit type juggling.  The strict comparison checks for both value and type equality, avoiding unexpected behavior.