# CSS Specificity Issue with !important and Inheritance

This repository demonstrates an uncommon CSS bug related to specificity, the `!important` declaration, and inheritance.  The `!important` declaration on a parent element unexpectedly affects a descendant element despite a more specific selector.

## Bug Description

A `!important` declaration on a parent element overrides a more specific selector on a descendant element, which is unexpected and can lead to inconsistent styling.

## How to Reproduce

1. Open `bug.css` and review the provided CSS code.
2. Inspect the styles applied to the `grandchild` element. Note that it inherits the `font-size` from the parent `child` element due to `!important` declaration overriding more specific selector.

## Solution

Review `bugSolution.css` for a resolution. Removing the `!important` declaration, or adopting better specificity rules, allows the cascade to work as intended.