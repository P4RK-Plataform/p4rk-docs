# P4RK Spacing & Grid Tokens

> Spacing scale, border radius, and responsive grid system for the P4RK platform.
> Managed as **Figma Variables** (FLOAT tokens) in the **P4RK DS** file.

---

## Overview

| Group | Count | Description |
|---|---|---|
| `space/*` | 11 | Spacing scale based on 8px unit |
| `radius/*` | 6 | Border radius tokens |
| `grid/*` | 15 | Grid specs for 3 breakpoints |
| **Total** | **32** | |

**Figma Collection:** `Spacing` (`VariableCollectionId:16:45`)
**Mode:** `Default`

---

## Spacing Scale

8px base unit with additional 2px and 4px for fine-tuning.

| Token | Value | Usage |
|---|---|---|
| `space/2xs` | 2px | Hairline spacing, borders |
| `space/xs` | 4px | Tight inner padding, icon gaps |
| `space/sm` | 8px | Default inner padding, small gaps |
| `space/md` | 16px | Standard component padding |
| `space/lg` | 24px | Section inner padding, card padding |
| `space/xl` | 32px | Section gaps, large padding |
| `space/2xl` | 48px | Major section spacing |
| `space/3xl` | 64px | Page section spacing |
| `space/4xl` | 96px | Hero/landing section spacing |
| `space/5xl` | 128px | Large hero padding |
| `space/6xl` | 160px | Maximum section spacing (Apple-inspired) |

### Scale Rationale

The scale follows a progression: `2 > 4 > 8 > 16 > 24 > 32 > 48 > 64 > 96 > 128 > 160`

- **2-8px**: Fine control for component internals
- **16-32px**: Standard UI spacing
- **48-96px**: Section-level spacing
- **128-160px**: Apple-style generous whitespace for landing pages

---

## Border Radius

| Token | Value | Usage |
|---|---|---|
| `radius/sm` | 4px | Tags, chips, small elements |
| `radius/md` | 8px | Inputs, buttons, default radius |
| `radius/lg` | 12px | Cards, modals |
| `radius/xl` | 16px | Large cards, hero sections |
| `radius/2xl` | 24px | Pills, floating elements |
| `radius/full` | 9999px | Circles, fully rounded |

---

## Grid System

12-column responsive grid across 3 breakpoints.

### Desktop (1440px)

| Property | Value | Token |
|---|---|---|
| Viewport width | 1440px | `grid/desktop-width` |
| Content max-width | 1200px | `grid/desktop-content` |
| Columns | 12 | `grid/desktop-columns` |
| Gutter | 24px | `grid/desktop-gutter` |
| Side margin | 120px | `grid/desktop-margin` |
| Column width | ~75.3px | (computed) |

### Tablet (768px)

| Property | Value | Token |
|---|---|---|
| Viewport width | 768px | `grid/tablet-width` |
| Content max-width | 720px | `grid/tablet-content` |
| Columns | 8 | `grid/tablet-columns` |
| Gutter | 16px | `grid/tablet-gutter` |
| Side margin | 24px | `grid/tablet-margin` |
| Column width | ~76px | (computed) |

### Mobile (375px)

| Property | Value | Token |
|---|---|---|
| Viewport width | 375px | `grid/mobile-width` |
| Content max-width | 343px | `grid/mobile-content` |
| Columns | 4 | `grid/mobile-columns` |
| Gutter | 12px | `grid/mobile-gutter` |
| Side margin | 16px | `grid/mobile-margin` |
| Column width | ~76.75px | (computed) |

### Breakpoint Summary

| Breakpoint | Width | Columns | Gutter | Content |
|---|---|---|---|---|
| Mobile | 375px | 4 | 12px | 343px |
| Tablet | 768px | 8 | 16px | 720px |
| Desktop | 1440px | 12 | 24px | 1200px |

---

## Usage Guidelines

### For Designers

1. **Always use spacing tokens** for padding, margins, and gaps
2. Use `space/md` (16px) as the default starting point
3. For landing pages, use `space/4xl` to `space/6xl` for generous Apple-style whitespace
4. Apply `radius/md` (8px) as the default border radius for most components
5. Use the grid variables to set up Figma layout grids on frames

### For Developers

```css
/* Example CSS custom properties */
--space-2xs: 2px;
--space-xs: 4px;
--space-sm: 8px;
--space-md: 16px;
--space-lg: 24px;
--space-xl: 32px;
--space-2xl: 48px;
--space-3xl: 64px;
--space-4xl: 96px;
--space-5xl: 128px;
--space-6xl: 160px;

--radius-sm: 4px;
--radius-md: 8px;
--radius-lg: 12px;
--radius-xl: 16px;
--radius-2xl: 24px;
--radius-full: 9999px;

/* Grid */
--grid-desktop-content: 1200px;
--grid-tablet-content: 720px;
--grid-mobile-content: 343px;
```

---

## References

- **Figma file:** [P4RK DS](https://www.figma.com/design/pJwPqZX9GycprKDfK3Ehec)
- **JSON tokens:** [`design-tokens.json`](./design-tokens.json)
- **Color tokens:** [`design-tokens.md`](./design-tokens.md)
- **Typography tokens:** [`typography-tokens.md`](./typography-tokens.md)
