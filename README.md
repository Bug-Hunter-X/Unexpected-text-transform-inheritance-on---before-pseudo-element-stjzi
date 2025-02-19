# Unexpected text-transform inheritance on ::before pseudo-element

This repository demonstrates a subtle CSS bug where the `text-transform` property unexpectedly affects the content of a `::before` pseudo-element due to inheritance.

The `bug.css` file contains the erroneous code. The `solution.css` file provides a solution to prevent this unexpected behavior.

## Bug Description:
The `text-transform: uppercase;` property applied to a parent element unexpectedly affects the content of its `::before` pseudo-element, converting the content to uppercase.

## Solution:
To avoid this, explicitly set the `text-transform` property to `none` on the pseudo-element or use a more specific selector and add `text-transform: none` there. 