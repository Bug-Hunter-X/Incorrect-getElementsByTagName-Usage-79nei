# Uncommon HTML Error: Incorrect getElementsByTagName Usage

This repository demonstrates a common error when working with `getElementsByTagName` in JavaScript within an HTML context.  The error arises from treating the NodeList returned by `getElementsByTagName` as a single element, rather than an array-like collection of elements.

## Bug Description
The `bug.html` file contains a simple HTML structure.  A script attempts to modify the `innerHTML` of a div element using `getElementsByTagName`. However, it incorrectly assumes `getElementsByTagName` returns a single element when it returns a NodeList. This leads to a runtime error.

## Solution
The `bugSolution.html` file demonstrates the correct approach. It properly accesses the element using its index or by using `getElementById` and then modifies the `innerHTML`.