---
name: Clinical Precision System
colors:
  surface: '#f9f9ff'
  surface-dim: '#d3daef'
  surface-bright: '#f9f9ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f1f3ff'
  surface-container: '#e9edff'
  surface-container-high: '#e1e8fd'
  surface-container-highest: '#dce2f7'
  on-surface: '#141b2b'
  on-surface-variant: '#3e4a3d'
  inverse-surface: '#293040'
  inverse-on-surface: '#edf0ff'
  outline: '#6e7b6c'
  outline-variant: '#bdcaba'
  surface-tint: '#006e2d'
  primary: '#006b2c'
  on-primary: '#ffffff'
  primary-container: '#00873a'
  on-primary-container: '#f7fff2'
  inverse-primary: '#62df7d'
  secondary: '#006a63'
  on-secondary: '#ffffff'
  secondary-container: '#99efe5'
  on-secondary-container: '#006f67'
  tertiary: '#a72d51'
  on-tertiary: '#ffffff'
  tertiary-container: '#c74668'
  on-tertiary-container: '#fffbff'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#7ffc97'
  primary-fixed-dim: '#62df7d'
  on-primary-fixed: '#002109'
  on-primary-fixed-variant: '#005320'
  secondary-fixed: '#9cf2e8'
  secondary-fixed-dim: '#80d5cb'
  on-secondary-fixed: '#00201d'
  on-secondary-fixed-variant: '#00504a'
  tertiary-fixed: '#ffd9de'
  tertiary-fixed-dim: '#ffb2bf'
  on-tertiary-fixed: '#3f0016'
  on-tertiary-fixed-variant: '#8a143c'
  background: '#f9f9ff'
  on-background: '#141b2b'
  surface-variant: '#dce2f7'
typography:
  page-title:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
    letterSpacing: -0.02em
  section-title:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '600'
    lineHeight: 28px
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  table-cell:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: '400'
    lineHeight: 18px
  caption:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
    letterSpacing: 0.01em
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
  container-margin: 24px
  gutter: 16px
  table-row-height: 44px
  compact-padding: 8px
  form-gap: 20px
---

## Brand & Style
The design system is engineered for high-stakes pharmaceutical environments where speed of recognition and operational accuracy are paramount. The visual narrative centers on **Corporate Modernism** with a heavy emphasis on **Functional Utility**. 

The aesthetic is characterized by a "White-Label Professionalism"—using ample whitespace, crisp borders, and a disciplined color application to reduce cognitive load during complex medication management workflows. The emotional response is one of calm authority, ensuring pharmacists and administrators feel supported by a stable, predictable interface.

## Colors
This design system utilizes a structured palette designed for rapid status scanning. 
- **Primary Green (#16A34A):** Reserved for primary actions and "Safe/Ready" states.
- **Secondary Teal (#0F766E):** Used for analytical overlays and secondary navigational accents.
- **Backgrounds:** The app background uses a cool gray (#F6F8FA) to provide subtle contrast against the pure white (#FFFFFF) surface cards, creating a clear physical distinction between the workspace and the container.
- **Status Semantic Mapping:** Every status must pair its specific color with a dedicated icon (e.g., Expiration uses Red + 'Alert' icon) to ensure accessibility for color-blind users in high-pressure clinical settings.

## Typography
The typography system relies exclusively on **Inter** to leverage its exceptional legibility at small sizes. 
- **Scale:** We prioritize a compact scale. Tables use 13px text to maximize data density without sacrificing readability.
- **Hierarchy:** Use `label-caps` for secondary metadata in headers or table headers to create clear separation from user-generated data.
- **Numerical Data:** For inventory counts and dosage values, ensure the use of tabular num-variants (tnum) to maintain vertical alignment in lists and tables.

## Layout & Spacing
The layout follows a **Fixed-Fluid Hybrid** model. The sidebar remains fixed at 260px (collapsible to 64px), while the main content area utilizes a fluid grid.
- **Enterprise Density:** A strict 4px/8px baseline grid is used. Form layouts on desktop must default to a 2-column span to reduce vertical scrolling.
- **Table Structure:** Enterprise tables use a fixed row height of 44px. Horizontal scrolling is permitted for wide datasets, with the first column (usually Medication Name or ID) locked to the left.
- **Breakpoints:** On tablets, the 2-column form reflows to a single column. The sidebar transitions to a drawer overlay on mobile devices.

## Elevation & Depth
This design system avoids heavy shadows to maintain a "clean-room" clinical feel. 
- **Flat Surface Tiering:** Depth is primarily communicated through background color shifts (Surface vs. App Background) and **Low-Contrast Outlines** (1px solid #E5E7EB).
- **Interactive Elevation:** Only floating elements (Modals, Popovers, Drawers) receive an ambient shadow (8px blur, 4% opacity, neutral tint) to signify they exist on a separate functional plane.
- **Focus States:** Active input fields and focused buttons use a 2px primary color ring with a 2px white offset.

## Shapes
The shape language is **Soft and Precise**. 
- **Standard Radius:** All buttons, inputs, and cards use a 4px (0.25rem) radius. This provides a modern touch while maintaining the structural rigidity expected of enterprise software.
- **Pill Variant:** Reserved exclusively for status "Chips" and "Tags" (e.g., EXPIRED, ACTIVE) to distinguish them from interactive buttons.

## Components

### Navigation
- **Sidebar:** Nested hierarchy with chevron indicators. Use a subtle active-state background (#F0FDF4) and a 3px left-border accent in Primary Green for the selected route.
- **Branch Selector:** Positioned in the Top Header as a searchable dropdown with a "Hospital/Location" icon.

### Buttons & Inputs
- **Primary:** Solid #16A34A with white text.
- **Secondary:** Solid #DCFCE7 with #16A34A text.
- **Forms:** Labels are always top-aligned. Autocomplete inputs must highlight the matching string in the results list. Date ranges should include "Quick Select" presets (Today, Last 7 Days, Near Expiry).

### Data & Pharmacy Specifics
- **High-Density Table:** Rows must change background color slightly on hover. Bulk selection checkboxes should appear in the first column.
- **Expiry Indicators:** Use a "Traffic Light" system within the table cells: Red text/icon for &lt;30 days, Amber for 30-90 days, Green for &gt;90 days.
- **FEFO Tags:** Inventory items should be tagged with a "First-Expiry-First-Out" badge in the batch selector to guide dispensing logic.
- **Unit Conversions:** Input fields for medication quantities should include a trailing unit label (e.g., "mg", "ml", "Tabs") that is non-editable but visually part of the field.

### Feedback
- **Notifications:** Toasts appear in the top-right. Success messages stay for 3 seconds; Error messages require manual dismissal.
- **Workflow Steppers:** Vertical steppers for mobile; Horizontal for desktop. Completed steps use a Green Checkmark; current steps use a Primary Border circle.