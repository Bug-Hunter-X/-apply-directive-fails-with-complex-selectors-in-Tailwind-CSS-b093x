# Bug Report: Tailwind CSS @apply Directive Failure

This repository demonstrates a bug where Tailwind CSS's `@apply` directive fails to apply styles correctly when the referenced class uses complex selectors, such as pseudo-classes or media queries.

## Bug Description

The `@apply` directive does not correctly apply styles defined in a class with a complex selector, like `:hover`, resulting in no visual changes upon interaction. 

## Reproduction Steps

1. Clone this repository.
2. Open `bug.css`.  Observe the `hover\:bg-red-500` class and its corresponding HTML in `index.html` (or similar).
3. Open `index.html` in a browser. 
4. Hover over the button; the background color will not change as expected. 

## Expected Behavior

The background color of the button should change to red upon hovering.

## Actual Behavior

The background color does not change.

## Solution

See `bugSolution.css` and associated `index.html` (if applicable) for a workaround.  This example avoids `@apply` for complex selectors.