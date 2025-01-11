# Tailwind CSS @apply Directive Issue with Pseudo-Selectors

This repository demonstrates a bug where Tailwind's `@apply` directive doesn't correctly apply styles with pseudo-selectors like `:hover`.

## Bug Description

When using `@apply` with a class containing `:hover` or similar selectors, the styles may not be applied correctly, leading to unexpected visual behavior.  This is especially problematic when trying to apply complex hover effects dynamically.

## How to Reproduce

1. Clone this repository.
2. Open `bug.html` in your browser.
3. Observe that the hover effect for the button is not applied correctly.

## Solution

The solution is to avoid using `@apply` with pseudo-selectors. Instead, apply the styles directly to the HTML element or use a utility-first approach.  Refer to `bugSolution.html` for a working example.