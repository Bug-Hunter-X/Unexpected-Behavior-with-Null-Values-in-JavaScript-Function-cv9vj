# Unexpected Behavior with Null Values in JavaScript

This repository demonstrates a common JavaScript bug related to how loose comparison handles null values. The `foo` function is intended to add two numbers, but its handling of null inputs leads to incorrect results. The `bug.js` file contains the buggy code, while `bugSolution.js` provides a corrected version.

## Bug Description
The original `foo` function uses loose comparison (`===`) to check for null values.  While this works for explicitly checking null, it masks potential issues with other falsy values (0, "", false, undefined). This can lead to unexpected outputs and errors in larger applications.