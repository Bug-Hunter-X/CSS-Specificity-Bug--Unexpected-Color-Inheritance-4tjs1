# CSS Specificity Bug: Unexpected Color Inheritance

This repository demonstrates a common CSS bug related to specificity and inheritance.  The `bug.css` file contains code where a child element's style is not properly overridden due to a conflict between `!important` declarations and CSS selector specificity.

The `bugSolution.css` file provides a solution that addresses the issue.

## Bug Description
The issue arises from a specificity conflict. While a more specific selector (`parent .child`) is used to try to override the style, the `!important` declaration in the less specific selector has higher precedence.

## Solution
The solution involves understanding and carefully managing CSS specificity.  The `bugSolution.css` file shows how to correct the problem using several strategies:

1. Removing the `!important` declarations where possible to increase predictability and maintainability.
2. Ensuring that more specific selectors are defined correctly in the CSS cascade.
3. When possible, using a more specific selector to set a more granular rule.
