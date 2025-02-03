# CSS Flexbox Overlap Bug

This repository demonstrates an uncommon bug related to flexbox behavior in CSS.  The issue involves inner divs unexpectedly overlapping instead of wrapping to the next line when the screen width reduces.  The solution provided addresses the problem by ensuring proper wrapping behavior.

## Bug Description

The original CSS uses flexbox to create a responsive layout.  However, on smaller screen sizes, the inner divs overlap vertically instead of wrapping horizontally. This unexpected behavior is inconsistent with typical flexbox behavior.

## Solution

The solution utilizes the `flex-wrap` property of flexbox to explicitly control the wrapping behavior of the flex items. Setting `flex-wrap: wrap` ensures that the items wrap onto multiple lines when necessary. The width of the flex items is made more dynamic to better adapt to screen size changes, using `flex-basis` for the initial width and allowing for a flexible spread of elements, preventing overlap.

## How to Reproduce

1. Clone this repository.
2. Open `bug.html` in a web browser.
3. Resize the browser window. Observe that the inner divs overlap below a certain breakpoint.
4. Open `bugSolution.html` to see the corrected behavior.