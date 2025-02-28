# Adaptive W3C 2025 logos

This folder contains versions of the 2025 W3C logos. See [W3C brand standards r5 version](https://lists.w3.org/Archives/Team/team-website-redesign/2024Dec/att-0005/W3C-Brand_Standards-r5.pdf) (*team-only*).

These logos, unlike the ones in [../w3c-2025/](../w3c-2025/), automatically adapt to their environment (currently only to dark color schemes).

In other words, if you have a page with a style sheet that adapts to dark mode (i.e., it contains <code>@media (prefers-color-scheme: dark)</code>), replace image links such as

> <code>.../w3c-2025/svg/w3c.svg</code>

with

> <code>.../w3c-2025<b>-auto</b>/svg/w3c.svg</code>

(The way this works is that the SVG code of the images contain [CSS
media queries](https://www.w3.org/TR/mediaqueries-5/).)

*Warning:* The required CSS media queries have draft status (as of February 2025). They are expected to remain stable, though, and are supported in recent browsers. (In older browsers, the images work like static images and do not adapt to dark mode.)