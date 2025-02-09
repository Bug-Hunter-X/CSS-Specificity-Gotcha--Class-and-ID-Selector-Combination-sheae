# CSS Specificity Gotcha: Class and ID Selector Combination

This repository demonstrates an uncommon issue related to CSS specificity when combining class and ID selectors within the same element. The behavior isn't always intuitive and can lead to unexpected results if not carefully considered.

## Problem
The `bug.css` file contains CSS code that showcases the issue.  The unexpected behavior arises from the interaction of the `.container`, `#container`, and `.container #container` selectors.  The intended behavior might not be achieved due to the order of selectors in the CSS and the way specificity is calculated.

## Solution
The solution, found in `bugSolution.css`, addresses the issue by clarifying the specificity and ensuring the intended styling is applied consistently.  Various strategies such as using more specific selectors or adjusting the order in the stylesheet to make the desired selector win can be used to correct this issue. See the comments in the solution file for detailed explanation.

## How to Reproduce
1. Clone this repository.
2. Open `bug.html` in a web browser to observe the unexpected behavior based on `bug.css`.
3. Switch the CSS import to `bugSolution.css` in the `bug.html` file and observe how the correct behavior is achieved.