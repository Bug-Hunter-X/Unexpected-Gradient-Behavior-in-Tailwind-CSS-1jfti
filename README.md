# Unexpected Gradient Behavior in Tailwind CSS

This repository demonstrates an unexpected gradient behavior in Tailwind CSS.  The gradient either doesn't render correctly, appears cut off, or is distorted in some way.  This issue is likely related to a conflict with other CSS rules or improper use of Tailwind's gradient utilities.

## Bug Report

The issue occurs when attempting to apply a linear gradient using `bg-gradient-to-r` and specifying colors `from-blue-500` and `to-purple-500`. The expected behavior is a smooth color transition from blue to purple. The actual behavior is that gradient is not rendered or distorted.

## Solution

The solution might involve:

1. **Specificity:** Ensuring that your Tailwind classes have sufficient specificity to override any conflicting styles.
2. **Parent Containers:** Checking for issues with parent containers that might be interfering with the gradient display (overflow: hidden, for example).
3. **CSS Order:** Verifying the order of your CSS rules to ensure the gradient styles are applied correctly.
4. **Plugin Conflicts:** Determining if any plugins are clashing with Tailwind's styling.
5. **Tailwind Configuration:** Examining Tailwind's configuration file (`tailwind.config.js`) to ensure there are no conflicting settings.

