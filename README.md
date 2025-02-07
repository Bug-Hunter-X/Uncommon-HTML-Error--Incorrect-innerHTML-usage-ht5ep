# Uncommon HTML Error: Incorrect innerHTML Usage

This repository demonstrates an uncommon error related to the use of `innerHTML` in HTML.  The error arises from attempting to set `innerHTML` to a non-string value.  The solution shows how to correctly use `innerHTML` by converting the value to a string before assignment.

## Bug
The `bug.html` file contains the problematic code where `innerHTML` is set to a number (123). This will result in unexpected behavior. Modern browsers might still render it correctly, but it's not best practice and can cause issues in older browsers or other contexts.

## Solution
The `bugSolution.html` file demonstrates the correct way to handle this situation.  Before setting `innerHTML`, the numeric value is converted to a string using `toString()` ensuring compatibility and avoiding errors.