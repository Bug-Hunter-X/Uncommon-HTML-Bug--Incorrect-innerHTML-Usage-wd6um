# Uncommon HTML Bug: Incorrect innerHTML Usage

This repository demonstrates a subtle bug related to the use of `innerHTML` in HTML.  The primary issue involves attempting to modify the `innerHTML` of an element that does not exist in the DOM, resulting in a silent error that is often hard to debug.

The `bug.html` file shows the erroneous code, and `bugSolution.html` provides the corrected version.

## Bug Description

The original code attempts to manipulate the `innerHTML` property of an element with the ID "nonExistentElement." However, this element is not defined in the HTML structure.  Modern browsers handle this without throwing an explicit error, making it difficult to identify the problem.

## Solution

The solution involves ensuring that the element you are targeting with `innerHTML` actually exists in the HTML before attempting to modify it.  This often involves proper error handling or checking for the element's existence.