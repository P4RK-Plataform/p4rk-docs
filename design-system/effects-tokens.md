# P4RK Shape & Effects Tokens

> Border widths, shadows, opacity, transitions, and z-index layers for the P4RK platform.
> Managed as **Figma Variables** (FLOAT tokens) in the **P4RK DS** file.

---

## Overview

| Group | Count | Description |
|---|---|---|
| `border-width/*` | 3 | Border thickness tokens |
| `opacity/*` | 5 | Opacity scale |
| `shadow/*` | 16 | Drop shadow parameters (4 shadows x 4 values) |
| `shadow/*-color` | 2 | Shadow color tokens (stored in **Colors** collection) |
| `transition/*` | 3 | Animation durations |
| `z-index/*` | 4 | Stacking order layers |
| **Total** | **31** | |

**Figma Collection:** `Shape & Effects` (`VariableCollectionId:16:179`)
**Mode:** `Default`

---

## Border Width

| Token | Value | Usage |
|---|---|---|
| `border-width/thin` | 1px | Default borders, dividers |
| `border-width/medium` | 2px | Focused inputs, active states |
| `border-width/thick` | 4px | Heavy emphasis, progress bars |

---

## Shadows

Apple-inspired subtle shadows with increasing elevation.

### Shadow SM
| Property | Value |
|---|---|
| X Offset | 0 |
| Y Offset | 1px |
| Blur | 2px |
| Spread | 0 |
| Color | `rgba(0, 0, 0, 0.05)` |
| **CSS** | `0 1px 2px rgba(0,0,0,0.05)` |
| **Usage** | Subtle cards, inputs |

### Shadow MD
| Property | Value |
|---|---|
| X Offset | 0 |
| Y Offset | 4px |
| Blur | 6px |
| Spread | -1px |
| Color | `rgba(0, 0, 0, 0.07)` |
| **CSS** | `0 4px 6px -1px rgba(0,0,0,0.07)` |
| **Usage** | Elevated cards, dropdowns |

### Shadow LG
| Property | Value |
|---|---|
| X Offset | 0 |
| Y Offset | 10px |
| Blur | 15px |
| Spread | -3px |
| Color | `rgba(0, 0, 0, 0.1)` |
| **CSS** | `0 10px 15px -3px rgba(0,0,0,0.1)` |
| **Usage** | Modals, floating panels |

### Shadow XL
| Property | Value |
|---|---|
| X Offset | 0 |
| Y Offset | 20px |
| Blur | 25px |
| Spread | -5px |
| Color | `rgba(0, 0, 0, 0.15)` |
| **CSS** | `0 20px 25px -5px rgba(0,0,0,0.15)` |
| **Usage** | Hero elements, featured cards |

### Shadow Color Tokens

These are COLOR-type variables stored in the **Colors** collection (not Shape & Effects) because they support Light/Dark mode switching.

| Token | Light Mode | Dark Mode | Usage |
|---|---|---|---|
| `shadow/sm-color` | `#0000000D` (5% black) | `#0000001A` (10% black) | Default card/input shadow color |
| `shadow/focus-color` | `#72BDE580` (50% blue-300) | `#2E96D180` (50% blue-500) | Focus ring glow color |

---

## Opacity

| Token | Value | Usage |
|---|---|---|
| `opacity/0` | 0% | Fully transparent / hidden |
| `opacity/25` | 25% | Subtle overlays, disabled states |
| `opacity/50` | 50% | Half transparent, loading states |
| `opacity/75` | 75% | Mostly opaque, active overlays |
| `opacity/100` | 100% | Fully opaque / default |

---

## Transitions

| Token | Value | Usage |
|---|---|---|
| `transition/fast` | 150ms | Hover states, toggles, micro-interactions |
| `transition/normal` | 300ms | Standard animations, page transitions |
| `transition/slow` | 500ms | Modal open/close, complex transitions |

### Easing

Use these durations with the following easing curves:
- **ease-out** (`cubic-bezier(0, 0, 0.2, 1)`) — Most UI animations
- **ease-in-out** (`cubic-bezier(0.4, 0, 0.2, 1)`) — Enter/exit transitions
- **ease-in** (`cubic-bezier(0.4, 0, 1, 1)`) — Exit-only animations

---

## Z-Index Layers

| Token | Value | Usage |
|---|---|---|
| `z-index/dropdown` | 1000 | Dropdowns, popovers, tooltips |
| `z-index/sticky` | 1020 | Sticky headers, floating navbars |
| `z-index/modal` | 1050 | Modals, dialogs, full-screen overlays |
| `z-index/toast` | 1080 | Toast notifications, alerts |

### Stacking Order

```
z-index/toast      (1080)  ████████████████████████████
z-index/modal      (1050)  ██████████████████████████
z-index/sticky     (1020)  ████████████████████████
z-index/dropdown   (1000)  ██████████████████████
Page content          (1)  ██
```

---

## Usage Guidelines

### For Designers

1. Apply shadow effects from the Figma Effect Styles (not manually)
2. Use `border-width/thin` (1px) as default — only use thicker for emphasis
3. Test shadows on both light and dark backgrounds

### For Developers

```css
/* Shadows */
--shadow-sm: 0 1px 2px rgba(0, 0, 0, 0.05);
--shadow-md: 0 4px 6px -1px rgba(0, 0, 0, 0.07);
--shadow-lg: 0 10px 15px -3px rgba(0, 0, 0, 0.1);
--shadow-xl: 0 20px 25px -5px rgba(0, 0, 0, 0.15);

/* Border widths */
--border-thin: 1px;
--border-medium: 2px;
--border-thick: 4px;

/* Transitions */
--transition-fast: 150ms ease-out;
--transition-normal: 300ms ease-out;
--transition-slow: 500ms ease-in-out;

/* Z-index */
--z-dropdown: 1000;
--z-sticky: 1020;
--z-modal: 1050;
--z-toast: 1080;
```

---

## References

- **Figma file:** [P4RK DS](https://www.figma.com/design/pJwPqZX9GycprKDfK3Ehec)
- **JSON tokens:** [`design-tokens.json`](./design-tokens.json)
- **Color tokens:** [`design-tokens.md`](./design-tokens.md)
- **Typography tokens:** [`typography-tokens.md`](./typography-tokens.md)
- **Spacing tokens:** [`spacing-tokens.md`](./spacing-tokens.md)
