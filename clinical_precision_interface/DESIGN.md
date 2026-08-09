---
name: Clinical Precision Interface
colors:
  surface: '#f8f9fa'
  surface-dim: '#d9dadb'
  surface-bright: '#f8f9fa'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f3f4f5'
  surface-container: '#edeeef'
  surface-container-high: '#e7e8e9'
  surface-container-highest: '#e1e3e4'
  on-surface: '#191c1d'
  on-surface-variant: '#42474f'
  inverse-surface: '#2e3132'
  inverse-on-surface: '#f0f1f2'
  outline: '#727780'
  outline-variant: '#c2c7d1'
  surface-tint: '#2d6197'
  primary: '#00355f'
  on-primary: '#ffffff'
  primary-container: '#0f4c81'
  on-primary-container: '#8ebdf9'
  inverse-primary: '#a0c9ff'
  secondary: '#006d39'
  on-secondary: '#ffffff'
  secondary-container: '#91f8ae'
  on-secondary-container: '#00743c'
  tertiary: '#2c3340'
  on-tertiary: '#ffffff'
  tertiary-container: '#434a57'
  on-tertiary-container: '#b3b9c9'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#d2e4ff'
  primary-fixed-dim: '#a0c9ff'
  on-primary-fixed: '#001c37'
  on-primary-fixed-variant: '#07497d'
  secondary-fixed: '#91f8ae'
  secondary-fixed-dim: '#75db94'
  on-secondary-fixed: '#00210d'
  on-secondary-fixed-variant: '#005229'
  tertiary-fixed: '#dce2f3'
  tertiary-fixed-dim: '#c0c7d6'
  on-tertiary-fixed: '#151c27'
  on-tertiary-fixed-variant: '#404754'
  background: '#f8f9fa'
  on-background: '#191c1d'
  surface-variant: '#e1e3e4'
typography:
  headline-lg:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
    letterSpacing: -0.01em
  headline-sm:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '600'
    lineHeight: 24px
  body-lg:
    fontFamily: Inter
    fontSize: 15px
    fontWeight: '400'
    lineHeight: 22px
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  body-sm:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: '400'
    lineHeight: 18px
  label-md:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
    letterSpacing: 0.02em
  label-sm:
    fontFamily: Inter
    fontSize: 11px
    fontWeight: '600'
    lineHeight: 14px
  data-mono:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: '500'
    lineHeight: 18px
    letterSpacing: -0.01em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 4px
  container-padding: 16px
  element-gap: 8px
  row-height-sm: 32px
  row-height-md: 40px
  sidebar-width: 240px
  grid-columns: '12'
  gutter: 16px
---

## Brand & Style

The design system is engineered for the high-stakes environment of pharmacy management. It prioritizes utility, speed of data entry, and cognitive clarity over decorative aesthetics. The brand personality is **authoritative, methodical, and unwavering**. 

The visual style follows a **Modern Corporate** approach with a focus on high information density. It utilizes a structured "sheet-based" architecture where data is organized into clearly defined functional zones. Visual noise is minimized by replacing heavy shadows with subtle 1px strokes, ensuring that pharmacists can navigate complex inventory and prescription data without distraction.

## Colors

The palette is rooted in professional healthcare archetypes. 

- **Primary (Deep Blue):** Used for primary actions, navigation headers, and active states to instill trust and stability.
- **Secondary (Emerald):** Representing health and pharmacy, used for "Complete" actions, stock-in indicators, and growth-related data points.
- **Neutrals:** A rigorous scale of grays. Backgrounds use a light-gray wash (`#F3F4F6`) to distinguish the work surface from the white containers (`#FFFFFF`).
- **Semantic Colors:** High-saturation tones used strictly for status indicators (e.g., "Out of Stock," "Expiring Soon," "High Priority").

## Typography

The typography system is optimized for **Vietnamese diacritics**, ensuring that accents do not overlap or feel cramped at small sizes. 

We utilize a **compact scale**. `Body-md (14px)` is the standard for most interface text, while `Body-sm (13px)` is reserved for high-density data tables and sidebars. Headings are intentionally kept small to save vertical space for content. For numerical data such as SKU numbers, stock counts, and prices, use a medium weight to ensure legibility against background strokes.

## Layout & Spacing

This design system employs a **Fixed-Fluid Hybrid Grid**. The sidebar remains fixed at 240px, while the main content area utilizes a 12-column fluid grid.

**Density Rules:**
- **Vertical Rhythm:** Follows a 4px baseline. Most components (inputs, buttons) should be 32px or 40px in height.
- **Margins:** Standard page margins are 16px to maximize the "data per square inch."
- **Tables:** Use "Condensed" rows (32px height) for inventory lists to allow more records to be visible without scrolling.
- **Breakpoints:** Optimized primarily for 1920x1080 and 1440x900 desktop resolutions. Tablet layouts should stack sidebars into a "hamburger" menu but maintain the high-density grid.

## Elevation & Depth

To maintain a professional, flat aesthetic, depth is communicated through **Tonal Layering** and **Subtle Outlines** rather than shadows.

- **Level 0 (Background):** `#F3F4F6` — The canvas on which the app sits.
- **Level 1 (Surface):** `#FFFFFF` — The main working card or container. Uses a 1px solid border (`#E5E7EB`).
- **Level 2 (Interaction):** Hover states use a subtle background tint (`#F9FAFB`) and a slightly darker border (`#D1D5DB`).
- **Overlays:** Modals and dropdowns use a very soft, high-diffusion shadow (8px blur, 5% opacity) to provide a "lifted" affordance without breaking the flat aesthetic.

## Shapes

The shape language is **Soft-Square**. 

- **Components:** Standard buttons, inputs, and cards use a 4px corner radius. This provides enough softness to be approachable while remaining "clinical" and organized.
- **Chips/Badges:** Use a slightly higher radius (6px) to distinguish them from actionable buttons.
- **Selections:** Selected items in a list use a 0px radius on the inner side to maintain the visual flow of the list stack.

## Components

### Buttons
- **Primary:** Solid `#0F4C81`, white text, 4px radius. 
- **Secondary/Outline:** 1px border `#D1D5DB`, text `#374151`, white background.
- **Destructive:** Solid `#DC2626` (only for irreversible actions like "Delete Prescription").

### Data Tables
The core of the system. 
- **Header:** Light gray background (`#F9FAFB`), semi-bold text, 1px bottom border.
- **Cells:** 32px height, 1px horizontal dividers only.
- **Interaction:** Row hover highlights in `#F3F4F6`.

### Form Inputs
- **Style:** 1px border `#D1D5DB`. Active/Focus state uses a 1px `#0F4C81` border with a subtle 2px outer blue glow.
- **Labels:** Always top-aligned, using `Label-md` style for maximum field visibility.

### Status Badges
- Small, uppercase text. 
- Use "Ghost" styling: Light background tint (10% opacity of the semantic color) with a dark text color of the same hue. This prevents the UI from becoming visually overwhelming with too many bright colors.

### Additional Components
- **Search Bar:** Large, prominent search with a leading icon for quick SKU/Patient lookup.
- **Stock Indicators:** Vertical progress bars within table cells to show inventory levels relative to "Min/Max" settings.