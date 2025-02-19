# CSS calc() Unexpected Behavior with Percentages and Viewport Units

This repository demonstrates a common issue with the CSS `calc()` function when using percentages and viewport units (vw, vh) together.  The calculation is performed only once, upon initial render, and isn't dynamically updated as the viewport size changes.

## Problem

The `calc()` function in CSS is powerful for dynamic calculations, however,  when combining percentages and viewport units (like `vw` or `vh`), the calculation is not recalculated responsively as the viewport changes. This can result in elements overflowing containers or unexpected layout shifts.

## Solution

The provided solution uses JavaScript to recalculate the width based on the viewport size. Although this approach adds a JavaScript dependency, it provides a reliable solution for dynamic responsiveness.