# P4RK Design Tokens

> Single source of truth for all color tokens used across the P4RK platform.
> Managed as Figma Variables in the **P4RK DS** file with Light and Dark mode support.

---

## Overview

| Category | Count | Description |
|---|---|---|
| Primary Blues | 6 | Brand colors anchored on P4RK blue |
| Neutrals | 12 | Grayscale from black to white |
| Success | 5 | Green feedback scale |
| Warning | 5 | Amber feedback scale |
| Error | 5 | Red feedback scale |
| Info | 5 | Blue feedback scale |
| Semantic Tokens | 23 | Context-aware tokens for UI elements |
| **Total** | **61** | |

---

## Figma Variable Collection

- **Collection name:** `Colors`
- **Modes:** `Light`, `Dark`
- **File:** P4RK DS (`pJwPqZX9GycprKDfK3Ehec`)

---

## Primary Blues

Core brand palette derived from the P4RK identity.

| Token | Light Mode | Dark Mode | Usage |
|---|---|---|---|
| `primary/blue-900` | `#1B4F72` | `#D4E6F1` | Primary brand, CTAs, headers |
| `primary/blue-700` | `#2E86C1` | `#85C1E9` | Links, hover states |
| `primary/blue-500` | `#3498DB` | `#3498DB` | General accent |
| `primary/blue-300` | `#85C1E9` | `#2E86C1` | Light accent, tags |
| `primary/blue-100` | `#D4E6F1` | `#1B4F72` | Subtle backgrounds |
| `primary/blue-50` | `#EBF5FB` | `#0D2737` | Very subtle tints |

---

## Neutrals

Grayscale used for text, backgrounds, borders, and structural elements.

| Token | Light Mode | Dark Mode |
|---|---|---|
| `black` | `#000000` | `#FFFFFF` |
| `gray-900` | `#111827` | `#F9FAFB` |
| `gray-800` | `#1F2937` | `#F3F4F6` |
| `gray-700` | `#374151` | `#E5E7EB` |
| `gray-600` | `#4B5563` | `#D1D5DB` |
| `gray-500` | `#6B7280` | `#9CA3AF` |
| `gray-400` | `#9CA3AF` | `#6B7280` |
| `gray-300` | `#D1D5DB` | `#4B5563` |
| `gray-200` | `#E5E7EB` | `#374151` |
| `gray-100` | `#F3F4F6` | `#1F2937` |
| `gray-50` | `#F9FAFB` | `#111827` |
| `white` | `#FFFFFF` | `#000000` |

---

## Feedback Colors

### Success

| Token | Light Mode | Dark Mode |
|---|---|---|
| `success-900` | `#14532D` | `#BBF7D0` |
| `success-700` | `#15803D` | `#86EFAC` |
| `success-500` | `#22C55E` | `#22C55E` |
| `success-300` | `#86EFAC` | `#15803D` |
| `success-100` | `#DCFCE7` | `#052E16` |

### Warning

| Token | Light Mode | Dark Mode |
|---|---|---|
| `warning-900` | `#78350F` | `#FDE68A` |
| `warning-700` | `#B45309` | `#FCD34D` |
| `warning-500` | `#F59E0B` | `#F59E0B` |
| `warning-300` | `#FCD34D` | `#B45309` |
| `warning-100` | `#FEF3C7` | `#451A03` |

### Error

| Token | Light Mode | Dark Mode |
|---|---|---|
| `error-900` | `#7F1D1D` | `#FECACA` |
| `error-700` | `#B91C1C` | `#FCA5A5` |
| `error-500` | `#EF4444` | `#EF4444` |
| `error-300` | `#FCA5A5` | `#B91C1C` |
| `error-100` | `#FEE2E2` | `#450A0A` |

### Info

| Token | Light Mode | Dark Mode |
|---|---|---|
| `info-900` | `#1E3A5F` | `#BFDBFE` |
| `info-700` | `#1D4ED8` | `#93C5FD` |
| `info-500` | `#3B82F6` | `#3B82F6` |
| `info-300` | `#93C5FD` | `#1D4ED8` |
| `info-100` | `#DBEAFE` | `#172554` |

---

## Semantic Tokens

Context-aware tokens that map to primitive colors. These are the tokens components should reference directly.

### Backgrounds & Surfaces

| Token | Light Mode | Dark Mode | Usage |
|---|---|---|---|
| `semantic/background` | `#FFFFFF` | `#0A0A0A` | Default page background |
| `semantic/background-secondary` | `#F9FAFB` | `#171717` | Secondary/subtle background |
| `semantic/surface` | `#FFFFFF` | `#1A1A1A` | Card and elevated surfaces |
| `semantic/surface-hover` | `#F3F4F6` | `#262626` | Surface hover state |
| `semantic/muted` | `#F3F4F6` | `#262626` | Tags, badges, muted areas |
| `semantic/overlay` | `#00000080` | `#00000099` | Modal/dialog overlay |

### Text & Foreground

| Token | Light Mode | Dark Mode | Usage |
|---|---|---|---|
| `semantic/foreground` | `#111827` | `#F9FAFB` | Primary text |
| `semantic/foreground-secondary` | `#6B7280` | `#9CA3AF` | Secondary/muted text |
| `semantic/foreground-tertiary` | `#9CA3AF` | `#6B7280` | Placeholder text |
| `semantic/foreground-inverse` | `#FFFFFF` | `#0A0A0A` | Text on dark/accent backgrounds |

### Borders

| Token | Light Mode | Dark Mode | Usage |
|---|---|---|---|
| `semantic/border` | `#E5E7EB` | `#2E2E2E` | Default border |
| `semantic/border-strong` | `#D1D5DB` | `#404040` | Focused/strong border |

### Accent (Brand)

| Token | Light Mode | Dark Mode | Usage |
|---|---|---|---|
| `semantic/accent` | `#1B4F72` | `#2E86C1` | Primary CTAs, links |
| `semantic/accent-hover` | `#2E86C1` | `#3498DB` | Accent hover state |
| `semantic/accent-muted` | `#D4E6F1` | `#1B4F72` | Subtle accent background |

### Feedback Semantics

| Token | Light Mode | Dark Mode | Usage |
|---|---|---|---|
| `semantic/success-bg` | `#DCFCE7` | `#052E16` | Success alert background |
| `semantic/success-text` | `#15803D` | `#86EFAC` | Success alert text |
| `semantic/warning-bg` | `#FEF3C7` | `#451A03` | Warning alert background |
| `semantic/warning-text` | `#B45309` | `#FCD34D` | Warning alert text |
| `semantic/error-bg` | `#FEE2E2` | `#450A0A` | Error alert background |
| `semantic/error-text` | `#B91C1C` | `#FCA5A5` | Error alert text |
| `semantic/info-bg` | `#DBEAFE` | `#172554` | Info alert background |
| `semantic/info-text` | `#1D4ED8` | `#93C5FD` | Info alert text |

---

## Usage Guidelines

### For Designers

1. **Always use semantic tokens** when styling components (e.g., use `semantic/foreground` instead of hardcoding `#111827`)
2. **Use primitive tokens** only when building new semantic tokens or for one-off decorative elements
3. **Test in both modes** by switching the Figma variable mode between Light and Dark
4. **Never hardcode hex values** in components; always bind fills/strokes to variables

### For Developers

1. Import `design-tokens.json` into your CSS/JS framework
2. Reference tokens by their semantic name: `var(--semantic-foreground)`
3. Implement mode switching via a `data-theme` attribute or CSS media query
4. See the companion `design-tokens.json` for machine-readable values

---

## References

- **Figma file:** [P4RK DS](https://www.figma.com/design/pJwPqZX9GycprKDfK3Ehec)
- **JSON tokens:** [`design-tokens.json`](./design-tokens.json)
- **Design inspiration:** apple.com, linear.app, stripe.com, vercel.com
