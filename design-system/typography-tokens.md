# P4RK Typography Tokens

> Typography scale and font hierarchy for the P4RK platform.
> Managed as Figma Text Styles in the **P4RK DS** file.

---

## Overview

| Category | Count | Description |
|---|---|---|
| Headings | 6 | H1 through H6, large display to section headers |
| Body | 3 | Body Large, Body, Body Small |
| Labels | 3 | Label Large, Label, Label Small |
| Caption & Overline | 2 | Small descriptive and uppercase text |
| Code | 2 | Monospace for technical content |
| **Total** | **16** | |

---

## Fonts

| Role | Family | Fallback Stack |
|---|---|---|
| Primary | **Inter** | `-apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif` |
| Code | **JetBrains Mono** | `"Fira Code", "SF Mono", Consolas, monospace` |

---

## Headings

Apple-inspired: large, bold, tight tracking for maximum impact.

| Token | Size | Weight | Line Height | Letter Spacing | Usage |
|---|---|---|---|---|---|
| `Heading/H1` | 72px | Bold (700) | 1.1 (79.2px) | -2px | Hero headlines, landing page |
| `Heading/H2` | 48px | Semi Bold (600) | 1.15 (55.2px) | -1.5px | Section titles |
| `Heading/H3` | 36px | Semi Bold (600) | 1.2 (43.2px) | -1px | Sub-section titles |
| `Heading/H4` | 28px | Semi Bold (600) | 1.2 (33.6px) | -0.5px | Card titles, feature headers |
| `Heading/H5` | 24px | Medium (500) | 1.25 (30px) | -0.3px | Sidebar headers, widget titles |
| `Heading/H6` | 20px | Medium (500) | 1.3 (26px) | -0.2px | Small section headers |

---

## Body

Clean and readable with generous line height for long-form content.

| Token | Size | Weight | Line Height | Letter Spacing | Usage |
|---|---|---|---|---|---|
| `Body/Body Large` | 18px | Regular (400) | 1.6 (28.8px) | 0 | Lead paragraphs, feature descriptions |
| `Body/Body` | 16px | Regular (400) | 1.5 (24px) | 0 | Default body text |
| `Body/Body Small` | 14px | Regular (400) | 1.5 (21px) | 0 | Secondary text, descriptions |

---

## Labels

Medium weight for actionable UI elements.

| Token | Size | Weight | Line Height | Letter Spacing | Usage |
|---|---|---|---|---|---|
| `Label/Label Large` | 16px | Medium (500) | 1.4 (22.4px) | 0 | Form labels, nav items |
| `Label/Label` | 14px | Medium (500) | 1.4 (19.6px) | 0 | Buttons, tabs, links |
| `Label/Label Small` | 12px | Medium (500) | 1.4 (16.8px) | +0.2px | Badges, tags, chips |

---

## Caption & Overline

Small text for supplementary information.

| Token | Size | Weight | Line Height | Letter Spacing | Usage |
|---|---|---|---|---|---|
| `Caption/Caption` | 12px | Regular (400) | 1.4 (16.8px) | +0.1px | Helper text, timestamps, footnotes |
| `Caption/Overline` | 11px | Medium (500) | 1.4 (15.4px) | +1.5px | Section overlines, uppercase labels |

---

## Code

Monospace for technical and developer-facing content.

| Token | Size | Weight | Line Height | Letter Spacing | Usage |
|---|---|---|---|---|---|
| `Code/Code` | 14px | Regular (400) | 1.6 (22.4px) | 0 | Inline code, code blocks |
| `Code/Code Small` | 12px | Regular (400) | 1.5 (18px) | 0 | Terminal output, small snippets |

---

## Design Principles

1. **Hierarchy through size and weight** — Not color. Headings use tighter letter-spacing for density; body uses open spacing for readability.
2. **Minimal weight variations** — Only Regular, Medium, Semi Bold, and Bold. No Thin/Light to keep things crisp.
3. **Generous line heights** — Body at 1.5-1.6 for comfortable reading; headings at 1.1-1.3 for compactness.
4. **Negative tracking on headings** — Apple-style tight letter-spacing makes large text feel premium.
5. **Positive tracking on small text** — Caption and Label Small use slight positive spacing for legibility at small sizes.

---

## Usage Guidelines

### For Designers

1. **Always apply a text style** instead of manually setting font properties
2. Use `H1` sparingly — only for hero sections and landing pages
3. Pair headings with body text for visual hierarchy
4. Use `Overline` for category labels above section titles
5. Use `Code` styles for any technical content (API keys, commands, etc.)

### For Developers

```css
/* Example CSS custom properties */
--font-heading: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
--font-code: 'JetBrains Mono', 'Fira Code', monospace;

--text-h1: 700 72px/1.1 var(--font-heading);
--text-h2: 600 48px/1.15 var(--font-heading);
--text-body: 400 16px/1.5 var(--font-heading);
--text-code: 400 14px/1.6 var(--font-code);
```

---

## References

- **Figma file:** [P4RK DS](https://www.figma.com/design/pJwPqZX9GycprKDfK3Ehec)
- **JSON tokens:** [`design-tokens.json`](./design-tokens.json)
- **Color tokens:** [`design-tokens.md`](./design-tokens.md)
