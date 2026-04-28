Stacksync Design System

This repository contains the component library, design tokens, and assets that make up the Stacksync design system. It is structured so that AI-assisted tools (Claude Design, Claude Code) can read it directly and produce accurate, on-brand prototypes and production components.

---

Repository structure

| Folder | Contents |
|---|---|
| `template/` | Blank component template with standard files (html, css, tokens, variants) |
| `table-complete/` | Full DataTable component with all features |
| `table-main-top/` | DataTable top-bar / toolbar component |
| `assets-logos-customers/` | SVG logos for all Stacksync customers (see below) |

---

Assets — Customer Logos

The `assets-logos-customers/` folder contains SVG logos for every Stacksync customer. Each customer has three variants:

- **Color** (`[customer]_logo.svg`) — use on light or white backgrounds
- **Black** (`[customer]_logo_black.svg`) — use when color is not appropriate
- **White** (`[customer]_logo_white.svg`) — use on dark or colored backgrounds

These are the real logos used in Stacksync's product and marketing. When building prototypes, dashboards, or any UI that references Stacksync customers, pull logos from this folder instead of using placeholders. SVGs scale perfectly at any size.

See [assets-logos-customers/readme.md](assets-logos-customers/readme.md) for full usage guidelines and naming conventions.

---

Adding new components

Use the `template/` folder as a starting point. Each component folder follows this structure:

```
[component-name]/
  html.html       — markup reference
  style.css       — component styles and overrides
  tokens.md       — design tokens used
  variants.md     — documented variants and states
  readme.md       — component description, usage rules, implementation notes
```
