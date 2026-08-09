---
name: Clinical Precision Ledger
colors:
  surface: '#f8f9ff'
  surface-dim: '#cbdbf5'
  surface-bright: '#f8f9ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#eff4ff'
  surface-container: '#e5eeff'
  surface-container-high: '#dce9ff'
  surface-container-highest: '#d3e4fe'
  on-surface: '#0b1c30'
  on-surface-variant: '#45464d'
  inverse-surface: '#213145'
  inverse-on-surface: '#eaf1ff'
  outline: '#76777d'
  outline-variant: '#c6c6cd'
  surface-tint: '#565e74'
  primary: '#000000'
  on-primary: '#ffffff'
  primary-container: '#131b2e'
  on-primary-container: '#7c839b'
  inverse-primary: '#bec6e0'
  secondary: '#006398'
  on-secondary: '#ffffff'
  secondary-container: '#5bb8fe'
  on-secondary-container: '#00476e'
  tertiary: '#000000'
  on-tertiary: '#ffffff'
  tertiary-container: '#191c1e'
  on-tertiary-container: '#818486'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#dae2fd'
  primary-fixed-dim: '#bec6e0'
  on-primary-fixed: '#131b2e'
  on-primary-fixed-variant: '#3f465c'
  secondary-fixed: '#cce5ff'
  secondary-fixed-dim: '#93ccff'
  on-secondary-fixed: '#001d31'
  on-secondary-fixed-variant: '#004b73'
  tertiary-fixed: '#e0e3e5'
  tertiary-fixed-dim: '#c4c7c9'
  on-tertiary-fixed: '#191c1e'
  on-tertiary-fixed-variant: '#444749'
  background: '#f8f9ff'
  on-background: '#0b1c30'
  surface-variant: '#d3e4fe'
typography:
  display-lg:
    fontFamily: Hanken Grotesk
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Hanken Grotesk
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  headline-sm:
    fontFamily: Hanken Grotesk
    fontSize: 18px
    fontWeight: '600'
    lineHeight: 24px
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
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
  data-mono:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
  label-caps:
    fontFamily: Inter
    fontSize: 11px
    fontWeight: '700'
    lineHeight: 12px
    letterSpacing: 0.05em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 4px
  container-padding: 24px
  gutter: 16px
  row-height-dense: 32px
  row-height-standard: 48px
---

## Brand & Style

The design system is engineered for the Stock Movement Ledger (SPMS), catering to healthcare logistics professionals who require absolute clarity and auditability. The brand personality is **authoritative, meticulous, and resilient**, prioritizing data integrity over decorative elements.

The visual style follows a **Corporate / Modern** approach with high-density information architecture. It leverages a "Systematic Minimalism" philosophy—where whitespace is used not just for aesthetics, but as a functional separator to reduce cognitive load during complex audit tasks. The interface must evoke a sense of trust and "clinical accuracy," ensuring that every stock movement is traceable and every status is immediately decodable.

## Colors

The palette is anchored by a deep slate primary color to provide a grounded, professional foundation. The secondary blue acts as the functional action color, used for navigation and primary interactions.

**Functional Color Mapping:**
- **Primary:** Navigation, headers, and high-emphasis text.
- **Secondary:** Interactive elements, links, and primary buttons.
- **Neutral:** Secondary text, borders, and disabled states.
- **Semantic Accents:** 
    - **Import:** Emerald green, signifying stock addition.
    - **Export:** Crimson red, signifying stock removal.
    - **Transfer:** Royal purple, signifying internal movement.
    - **Adjustment:** Burnt orange, signifying corrections or audits.

## Typography

This design system utilizes a tiered typography strategy to manage high-density data. **Hanken Grotesk** is reserved for structural headings, providing a modern, sharp edge to the interface. **Inter** serves as the primary workhorse for body text and form inputs due to its exceptional legibility at small sizes.

For the Stock Movement Ledger, **JetBrains Mono** is introduced for all numeric data, batch numbers, and stock codes. This ensures that characters are easily distinguishable (e.g., '0' vs 'O') and columns of numbers align perfectly for visual scanning.

## Layout & Spacing

The layout utilizes a **Fixed Grid** system for the primary dashboard (1280px max-width) and a **Fluid Grid** for the data ledger tables to maximize screen real estate. 

**Spacing Principles:**
- **High-Density Tables:** Use a 4px baseline grid. Table rows should have a `row-height-dense` of 32px to allow as many records as possible above the fold.
- **Audit Sidebars:** Details regarding specific movements should emerge in a right-aligned drawer (400px fixed width), maintaining context of the main list.
- **Breakpoints:** 
    - Desktop: 1200px+ (12 columns, 24px margins)
    - Tablet: 768px - 1199px (8 columns, 16px margins)
    - Mobile: Below 768px (4 columns, 12px margins; switch ledger to card-view).

## Elevation & Depth

To maintain a "clinical" feel, the design system avoids heavy shadows. Instead, it utilizes **Tonal Layers** and **Low-contrast outlines**.

- **Surface Level 0 (Background):** Slate-50 (#F8FAFC).
- **Surface Level 1 (Table/Card):** Pure White (#FFFFFF) with a 1px border (#E2E8F0).
- **Surface Level 2 (Popovers/Drawers):** Pure White with a soft 8px blur, 4% opacity black shadow to suggest subtle lift.
- **Audit Trails:** Indicated by a vertical "track" line in the sidebar, using a solid 2px neutral-200 border to connect chronological nodes.

## Shapes

The shape language is **Soft (0.25rem)**. In a healthcare and data-heavy environment, sharp corners are avoided to reduce visual harshness, but excessive rounding is shunned to maintain a precise, space-efficient footprint.

- **Inputs and Buttons:** 4px radius.
- **Badges/Status Tags:** Fully rounded (pill) to distinguish them immediately from structural elements like buttons.
- **Data Containers:** 8px radius (`rounded-lg`) for major sections like ledger cards or summary panels.

## Components

### Data Tables
The core of the ledger. Use a fixed header on scroll. Column headers should be `label-caps` with a subtle grey background. Row hover states should use a 2% secondary color tint to track the horizontal eye-line.

### Status Badges
- **Import:** Emerald background (10% opacity) with Emerald-700 text.
- **Export:** Red background (10% opacity) with Red-700 text.
- **Transfer:** Purple background (10% opacity) with Purple-700 text.
- **Adjustment:** Orange background (10% opacity) with Orange-700 text.
*All badges include a 4px solid dot of the respective color to the left of the label.*

### Audit Trail Markers
Chronological events are marked with a circular node. If an entry is "Verified," the node contains a checkmark; if "Pending," it is a hollow ring.

### Input Fields
Utilize "Inter" at 14px. Labels are always visible (not floating) to ensure speed of data entry. Error states must be indicated by a 2px left-border accent in Red-600 in addition to the standard border color change.

### Buttons
- **Primary:** Solid Primary color with white text.
- **Secondary:** White background with 1px border.
- **Icon-Only:** Used for "View Details" or "Download Receipt" within table rows to save space.