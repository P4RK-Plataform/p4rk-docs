# P4RK Design Tokens

> Single source of truth for all design tokens used across the P4RK platform.
> Managed as Figma Variables and Text Styles in the **P4RK DS** file.

---

## Design System Overview

| Collection | Tokens | Figma Type | Documentation |
|---|---|---|---|
| **Colors** | 67 | Variables (COLOR) | This file |
| **Typography** | 42 + 16 styles | Variables (FLOAT) + Text Styles | [`typography-tokens.md`](./typography-tokens.md) |
| **Spacing** | 32 | Variables (FLOAT) | [`spacing-tokens.md`](./spacing-tokens.md) |
| **Shape & Effects** | 31 | Variables (FLOAT) | [`effects-tokens.md`](./effects-tokens.md) |
| **Components** | 76 | Variables (COLOR + FLOAT) | This file (Button + Form Input sections) |
| **Total** | **248** | | |

**JSON source:** [`design-tokens.json`](./design-tokens.json)

---

## Color Tokens Overview

| Category | Count | Description |
|---|---|---|
| Primary Blues | 6 | Brand colors anchored on PANTONE 2154 C (#004680) |
| Brand Grays | 4 | Brand gray scale from PANTONE Cool Gray 6 C (#A7A8AA) |
| Neutrals | 12 | Grayscale from black to white |
| Success | 5 | Green feedback scale |
| Warning | 5 | Amber feedback scale |
| Error | 5 | Red feedback scale |
| Info | 5 | Blue feedback scale |
| Semantic Tokens | 23 | Context-aware tokens for UI elements |
| Shadow Colors | 2 | Shadow color tokens (sm-color, focus-color) |
| **Total** | **67** | |

---

## Figma Variable Collection

- **Collection name:** `Colors`
- **Modes:** `Light`, `Dark`
- **File:** P4RK DS (`pJwPqZX9GycprKDfK3Ehec`)

---

## Primary Blues — PANTONE 2154 C

Core brand palette anchored on **PANTONE 2154 C** (`#004680`).

| Token | Light Mode | Dark Mode | Usage |
|---|---|---|---|
| `primary/blue-900` | `#004680` | `#E1F0FA` | Primary brand, CTAs, headers |
| `primary/blue-700` | `#0A6DB5` | `#72BDE5` | Links, hover states |
| `primary/blue-500` | `#2E96D1` | `#2E96D1` | General accent |
| `primary/blue-300` | `#72BDE5` | `#0A6DB5` | Light accent, tags |
| `primary/blue-100` | `#BFE0F5` | `#004680` | Subtle backgrounds |
| `primary/blue-50` | `#E5F2FB` | `#003459` | Very subtle tints |

---

## Brand Grays — PANTONE Cool Gray 6 C

Secondary brand color from **PANTONE Cool Gray 6 C** (`#A7A8AA`). Used for P, R, K letters in the logo and as a brand-specific neutral.

| Token | Light Mode | Dark Mode | Usage |
|---|---|---|---|
| `primary/gray-700` | `#A7A8AA` | `#A7A8AA` | Brand gray, logo letters |
| `primary/gray-500` | `#C4C5C6` | `#787979` | Lighter brand gray |
| `primary/gray-300` | `#DCDCDD` | `#5A5B5C` | Subtle brand gray |
| `primary/gray-100` | `#EFEFEF` | `#3D3D3E` | Background tint |

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
| `semantic/accent` | `#004680` | `#0A6DB5` | Primary CTAs, links |
| `semantic/accent-hover` | `#0A6DB5` | `#2E96D1` | Accent hover state |
| `semantic/accent-muted` | `#BFE0F5` | `#004680` | Subtle accent background |

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

## Button Component Tokens

Component-level tokens for the button system. Stored in the **Components** Figma Variable collection (`VariableCollectionId:34:1019`) with Light/Dark modes.

### Variants

| Variant | Description | Usage |
|---|---|---|
| **Primary** | Solid blue fill | Main CTAs, form submits |
| **Secondary** | Outline with border | Secondary actions, cancel |
| **Ghost** | Text only, no fill/border | Tertiary actions, inline links |
| **Destructive** | Solid red fill | Delete, remove, danger actions |

### Button Color Tokens

#### Primary

| Token | Light Mode | Dark Mode |
|---|---|---|
| `button/primary-bg` | `#004680` | `#0A6DB5` |
| `button/primary-bg-hover` | `#0A6DB5` | `#2E96D1` |
| `button/primary-bg-active` | `#003459` | `#004680` |
| `button/primary-text` | `#FFFFFF` | `#FFFFFF` |

#### Secondary (Outline)

| Token | Light Mode | Dark Mode |
|---|---|---|
| `button/secondary-bg` | `#FFFFFF` | `#0A0A0A` |
| `button/secondary-bg-hover` | `#E5F2FB` | `#003459` |
| `button/secondary-border` | `#004680` | `#0A6DB5` |
| `button/secondary-text` | `#004680` | `#0A6DB5` |

#### Ghost

| Token | Light Mode | Dark Mode |
|---|---|---|
| `button/ghost-bg-hover` | `#F3F4F6` | `#1F2937` |
| `button/ghost-text` | `#111827` | `#F9FAFB` |

#### Destructive

| Token | Light Mode | Dark Mode |
|---|---|---|
| `button/destructive-bg` | `#B91C1C` | `#B91C1C` |
| `button/destructive-bg-hover` | `#7F1D1D` | `#EF4444` |
| `button/destructive-bg-active` | `#7F1D1D` | `#B91C1C` |
| `button/destructive-text` | `#FFFFFF` | `#FFFFFF` |

#### Shared

| Token | Light Mode | Dark Mode | Usage |
|---|---|---|---|
| `button/disabled-bg` | `#F3F4F6` | `#1F2937` | All disabled buttons background |
| `button/disabled-text` | `#9CA3AF` | `#6B7280` | All disabled buttons text |
| `button/disabled-border` | `#E5E7EB` | `#374151` | Disabled outline button border |
| `button/focus-ring` | `#72BDE5` | `#2E96D1` | Focus ring for all variants |

### Button Size Tokens

| Token | sm | md | lg |
|---|---|---|---|
| `button/{size}-height` | 36px | 44px | 52px |
| `button/{size}-padding-x` | 12px | 16px | 24px |
| `button/{size}-padding-y` | 6px | 8px | 12px |
| `button/{size}-font-size` | 14px | 16px | 16px |
| `button/{size}-icon-size` | 16px | 20px | 24px |
| `button/{size}-gap` | 6px | 8px | 8px |

### Shared Button Properties

| Property | Token Reference | Collection | Value |
|---|---|---|---|
| Border radius | `radius/md` | Spacing | 8px |
| Border width (outline) | `border-width/thin` | Shape & Effects | 1px |
| Font weight | `font-weight/medium` | Typography | 500 |
| Font family | Inter | — | — |
| Transition | `transition/fast` | Shape & Effects | 150ms |
| Focus ring width | `border-width/medium` | Shape & Effects | 2px |

### Figma Bindings

All button properties in the Figma showcase frame are bound to variables — zero hardcoded values:

| Property | Bound To |
|---|---|
| Fill colors | `button/*` COLOR tokens (Components) |
| Text colors | `button/*` COLOR tokens (Components) |
| Stroke colors | `button/*` COLOR tokens (Components) |
| Padding (L/R/T/B) | `button/{size}-padding-x/y` (Components) |
| Gap | `button/{size}-gap` (Components) |
| Font size | `button/{size}-font-size` (Components) |
| Corner radius | `radius/md` (Spacing) |
| Height | `button/{size}-height` (Components) |
| Shadow color | `shadow/sm-color` (Colors) |
| Shadow offsets | `shadow/sm-x`, `shadow/sm-y`, `shadow/sm-blur`, `shadow/sm-spread` (Shape & Effects) |
| Icon width/height | `button/{size}-icon-size` (Components) |
| Line height | `line-height/*` (Typography) |
| Letter spacing | `letter-spacing/*` (Typography) |
| Stroke weight | `border-width/thin` (Shape & Effects) |

### Icon Buttons

Square buttons using height as width. Available in all variants (Primary, Secondary/Outline, Ghost) and all sizes (sm=36x36, md=44x44, lg=52x52).

### Buttons with Icons

Support leading and trailing icons with `gap` spacing between icon and text. Icon size follows the size token (`button/{size}-icon-size`).

### Icon Components (Swappable)

All icons in buttons use **component instances** from the `Icon Placeholders` set. This allows swapping the entire icon library without rebuilding buttons.

| Component | Placeholder | Usage |
|---|---|---|
| `icon/arrow-right` | → | Next, forward navigation |
| `icon/arrow-left` | ← | Back, previous navigation |
| `icon/plus` | + | Create, add actions |
| `icon/close` | ✕ | Close, remove, delete |
| `icon/download` | ↓ | Download, export actions |

**Internal layer name:** All icon components use `glyph` as the internal text layer name. This ensures color overrides (token bindings) are preserved when swapping instances.

**How to swap icons:**
1. Double-click into a button to select the icon instance
2. Right-click → "Swap instance" → choose from your icon library
3. Color token bindings are preserved automatically

**When importing a new icon library:** Replace the content inside each `icon/*` master component, and every instance across the file updates automatically.

---

## Form Input Component Tokens

Component-level tokens for the form input system. Stored in the **Components** Figma Variable collection (`VariableCollectionId:34:1019`) with Light/Dark modes.

### Components

| Component | Description | Usage |
|---|---|---|
| **Text Input** | Single-line text field | Email, name, URL fields |
| **Textarea** | Multi-line text field | Messages, descriptions, comments |
| **Select / Dropdown** | Dropdown selector with chevron | Country, category selection |
| **Checkbox** | Square toggle with checkmark | Terms acceptance, multi-select options |
| **Radio Buttons** | Circular single-select | Exclusive option groups |
| **Toggle Switch** | Slide toggle with knob | On/off settings, feature flags |
| **Date Picker** | Date input with calendar icon | Start/end dates, scheduling |
| **Search Bar** | Input with search icon | Global search, filtering |

### States

All components support 5 states: **default**, **focus**, **error**, **success**, **disabled**.

### Form Input Color Tokens

| Token | Light Mode | Dark Mode | Usage |
|---|---|---|---|
| `input/bg` | `#FFFFFF` | `#1A1A1A` | Input background |
| `input/bg-disabled` | `#F3F4F6` | `#1F2937` | Disabled input background |
| `input/border` | `#E5E7EB` | `#2E2E2E` | Default border |
| `input/border-focus` | `#004680` | `#0A6DB5` | Focused border |
| `input/border-error` | `#B91C1C` | `#FCA5A5` | Error border |
| `input/border-success` | `#15803D` | `#86EFAC` | Success border |
| `input/border-disabled` | `#E5E7EB` | `#374151` | Disabled border |
| `input/text` | `#111827` | `#F9FAFB` | Input value text |
| `input/text-placeholder` | `#6B7280` | `#9CA3AF` | Placeholder text |
| `input/text-disabled` | `#9CA3AF` | `#6B7280` | Disabled text |
| `input/label` | `#111827` | `#F9FAFB` | Field label |
| `input/helper` | `#6B7280` | `#9CA3AF` | Helper text |
| `input/error-text` | `#B91C1C` | `#FCA5A5` | Error message |
| `input/success-text` | `#15803D` | `#86EFAC` | Success message |
| `input/toggle-bg` | `#D1D5DB` | `#4B5563` | Toggle off track |
| `input/toggle-bg-on` | `#004680` | `#0A6DB5` | Toggle on track |
| `input/toggle-knob` | `#FFFFFF` | `#FFFFFF` | Toggle knob |
| `input/checkbox-bg` | `#004680` | `#0A6DB5` | Checked checkbox/radio |
| `input/checkbox-check` | `#FFFFFF` | `#FFFFFF` | Checkmark color |

### Form Input Size Tokens

| Token | Value | Usage |
|---|---|---|
| `input/height-sm` | 36px | Small input height |
| `input/height-md` | 44px | Medium input height (default) |
| `input/height-lg` | 52px | Large input height |
| `input/padding-x` | 12px | Horizontal padding |
| `input/padding-y` | 10px | Vertical padding |
| `input/font-size` | 14px | Input text font size |
| `input/label-font-size` | 14px | Label font size |
| `input/helper-font-size` | 12px | Helper/error text font size |
| `input/label-gap` | 6px | Gap between label and input |
| `input/helper-gap` | 4px | Gap between input and helper |
| `input/textarea-min-height` | 120px | Minimum textarea height |
| `input/toggle-width` | 44px | Toggle switch width |
| `input/toggle-height` | 24px | Toggle switch height |
| `input/toggle-knob-size` | 20px | Toggle knob diameter |
| `input/checkbox-size` | 20px | Checkbox/radio size |
| `input/icon-size` | 16px | Trailing/leading icon size |
| `input/close-icon-size` | 12px | Close/clear icon size in search bar |
| `input/width-sm` | 140px | Small input width (date picker, compact fields) |
| `input/width-md` | 170px | Medium input width (state showcase fields) |
| `input/width-lg` | 220px | Large input width (full-size fields) |
| `input/gap` | 8px | Gap between icon and text inside input |

### Shared Form Input Properties

| Property | Token Reference | Collection | Value |
|---|---|---|---|
| Border radius | `radius/md` | Spacing | 8px |
| Border width (default) | `border-width/thin` | Shape & Effects | 1px |
| Border width (focus) | `border-width/medium` | Shape & Effects | 2px |
| Checkbox radius | `radius/sm` | Spacing | 4px |
| Toggle radius | `radius/full` | Spacing | 9999px |
| Font weight (input) | `font-weight/regular` | Typography | 400 |
| Font weight (label) | `font-weight/medium` | Typography | 500 |
| Font family | Inter | — | — |
| Transition | `transition/fast` | Shape & Effects | 150ms |

### Figma Bindings

All form input properties in the Figma showcase frame are bound to variables — zero hardcoded values:

| Property | Bound To |
|---|---|
| Fill colors | `input/*` COLOR tokens (Components) |
| Text colors | `input/*` COLOR tokens (Components) |
| Stroke colors | `input/*` COLOR tokens (Components) |
| Padding (L/R/T/B) | `input/padding-x/y` (Components) |
| Gap (icon ↔ text) | `input/gap` (Components) |
| Font size | `input/font-size`, `input/label-font-size`, `input/helper-font-size` (Components) |
| Corner radius | `radius/md`, `radius/sm`, `radius/full` (Spacing) |
| Height | `input/height-sm/md/lg` (Components) |
| Width | `input/width-sm/md/lg` (Components) |
| Shadow color | `shadow/sm-color`, `shadow/focus-color` (Colors) |
| Shadow offsets | `shadow/sm-*` (Shape & Effects) |
| Icon width/height | `input/icon-size`, `input/close-icon-size` (Components) |
| Line height | `line-height/*` (Typography) |
| Letter spacing | `letter-spacing/*` (Typography) |
| Stroke weight | `border-width/thin`, `border-width/medium` (Shape & Effects) |

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
- **Typography tokens:** [`typography-tokens.md`](./typography-tokens.md)
- **Spacing tokens:** [`spacing-tokens.md`](./spacing-tokens.md)
- **Effects tokens:** [`effects-tokens.md`](./effects-tokens.md)
- **Logo SVGs:** [`logos/`](./logos/)
- **Design inspiration:** apple.com, linear.app, stripe.com, vercel.com
