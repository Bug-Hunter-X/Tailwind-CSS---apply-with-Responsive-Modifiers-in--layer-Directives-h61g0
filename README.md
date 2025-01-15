# Tailwind CSS: @apply with Responsive Modifiers in @layer Directives

This repository demonstrates a bug where Tailwind CSS's `@apply` directive doesn't correctly apply responsive modifiers when used within `@layer` directives. The bug specifically impacts styles applied at larger breakpoints.

## Bug Description

The core problem is that Tailwind's `@apply` directive inside an `@layer`  fails to properly handle responsive modifiers such as `md:`, `lg:`, etc.  While the base styles might be applied, the responsive variations are often ignored.

## Reproduction Steps

1. Clone this repository.
2. Install Node.js and npm (or yarn).
3. Run `npm install` or `yarn install` to install dependencies (PostCSS and Tailwind).
4. Observe that the styles in `bug.css` do not apply correctly at the defined breakpoints.