# Flexbox Overflow Bug

This repository demonstrates a common issue with CSS flexbox layout where setting a percentage width on flex items doesn't account for padding, margins, or borders, leading to unexpected overflow or collapse when content is larger than expected.  The bug and solution are presented in separate CSS files.

## Bug
The `bug.css` file contains the erroneous CSS. The issue arises when the content within the `.item` elements exceeds the available space due to the unaccounted for padding, margin, and border contributions.

## Solution
The `bugSolution.css` file demonstrates the solution.  By using `box-sizing: border-box;` on the `.item` elements, padding and borders are included within the 50% width, preventing the overflow issue.