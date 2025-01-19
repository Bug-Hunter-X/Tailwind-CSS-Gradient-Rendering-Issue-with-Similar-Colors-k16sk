# Tailwind CSS Gradient Subtlety Issue

This repository demonstrates a subtle issue with Tailwind CSS gradients where similar `from` and `to` colors might render as a solid color depending on the display device and browser.  This isn't a bug in Tailwind, but rather a consequence of how color gradients are processed and displayed.

## Problem

The `bug.html` file contains a simple div with a gradient background. If the `from` and `to` colors are too close in hue, saturation, and brightness, the gradient might appear as a solid color.  This is more likely to happen on devices with limited color capabilities.

## Solution

The `solution.html` file offers possible solutions:

1.  Use colors with a greater degree of difference.  More contrasting colors generally produce more noticeable gradients.
2.  Consider alternative background styles if a gradient isn't critical to the design.
3.  Use a different gradient function like `linear-gradient` from pure CSS if more control is needed.  This provides more options but requires writing CSS instead of using the Tailwind utility classes.
