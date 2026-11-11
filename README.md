# Navigation Test Bloomington

Rivet sidebar navigation prototype for IU Bloomington. One self-contained page (`index.html`) plus an `assets/` folder. No build step.

- **Design:** Figma "Sidebar Designs" → Homepage frame
- **Components:** Rivet 3 Component Guide (spacing, type, hovers); tokens in `assets/rivet-tokens.css` are a copy of the guide's generated file
- **Sidebar behavior:** ported from `prototype-hub/v1.1/sidebar-v2-children`
- **Live:** https://manselldesign.github.io/navigation-test-bloomington/

## Where to edit

| What | Where in `index.html` |
| --- | --- |
| Navigation items (IA) | the `IA` list in the script at the bottom |
| Homepage copy and sections | `<template id="tpl-home">` |
| Colors, type, spacing | the `:root` tokens and "NAMED TEXT STYLES" at the top of the stylesheet |
| Content max width (1340px) | `--content-max` |
| Desktop / mobile split (1024px) | `SIDENAV_BREAKPOINT` and the two matching media queries |

## Layout rules

- Header spans the full window. The sidebar (260px) stays locked to the left under it.
- Each section's background fills the space to the right of the sidebar; its contents stop at 1340px and center in that space.
- Photos never grow past their Figma size (hero and image hub 1244px, billboard 800px).
- The footer fills the full width to the right of the sidebar.

## Placeholders to replace

- Second- and third-level navigation labels (Figma only defines the top level).
- Interior pages (only the homepage is designed).
- Large photos (`hero`, `hub-*`, `billboard`) are 1x renders from Figma; swap in full-resolution exports with the same file names.
