# Inconsistent Element Hiding in HTML using display and visibility

This repository demonstrates a subtle bug related to hiding HTML elements using CSS. The problem arises from using both `display: none;` and `visibility: hidden;` simultaneously.

While individually they can hide an element, using both together does not guarantee consistent results across all browsers.  Some browsers might render the element hidden, while others may not, leading to unexpected behavior.

## Bug

The `bug.html` file contains the buggy code. The `div` with the id "myDiv" is intended to be hidden, but due to the conflicting styles, it may or may not be hidden depending on the browser.

## Solution

The `bugSolution.html` file demonstrates the corrected approach. To reliably hide an element, you should only use one style property, either `display: none;` or `visibility: hidden;`, depending on the desired effect.
