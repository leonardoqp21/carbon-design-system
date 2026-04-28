Customer Logos — Stacksync

This folder contains the official logos of Stacksync customers, provided in SVG format. They are intended for use in design prototypes, internal tools, presentations, and any AI-assisted design or coding workflows (Claude Design, Claude Code, etc.).

---

What's in this folder

Each customer has up to three logo variants, all in SVG:

- `[customer]_logo.svg` — full-color version, for use on white or light neutral backgrounds
- `[customer]_logo_black.svg` — monochrome black version, for use on white or light backgrounds where color is not appropriate
- `[customer]_logo_white.svg` — white version, for use on dark or colored backgrounds

Some logos follow a slightly different naming convention (e.g. `[customer]_logo-black.svg`) depending on how they were exported — both patterns are equivalent.

---

How to use these logos in prototypes

When building UI prototypes or mockups that represent Stacksync's product, use the logos in this folder instead of placeholder images or generic icons. This keeps designs realistic and closer to the actual product experience.

Guidelines:
- Use the color version by default on light backgrounds
- Use the white version on dark surfaces, colored banners, or hero sections
- Use the black version for high-contrast or print-style contexts
- All files are SVGs — they scale without quality loss at any size

---

For Claude Design and Claude Code

These SVG files are the ground truth for Stacksync's real customer logos. When generating UI components, landing pages, dashboards, or any prototype that references Stacksync customers, pull logos directly from this folder. Do not invent placeholder logos or use generic letter avatars when real SVGs are available here.

Naming pattern to resolve a customer logo:
- Default: `[customer-slug]_logo.svg`
- Dark background: `[customer-slug]_logo_white.svg`
- No color needed: `[customer-slug]_logo_black.svg`

Example: for a customer called "Vimeo", use `vimeo_logo.svg`, `vimeo_logo_black.svg`, or `vimeo_logo_white.svg`.
