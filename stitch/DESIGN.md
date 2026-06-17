---
name: TaskBeacon Mini
colors:
  surface: '#fcf8fa'
  surface-dim: '#dcd9db'
  surface-bright: '#fcf8fa'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f6f3f5'
  surface-container: '#f0edef'
  surface-container-high: '#eae7e9'
  surface-container-highest: '#e4e2e4'
  on-surface: '#1b1b1d'
  on-surface-variant: '#45464d'
  inverse-surface: '#303032'
  inverse-on-surface: '#f3f0f2'
  outline: '#76777d'
  outline-variant: '#c6c6cd'
  surface-tint: '#565e74'
  primary: '#000000'
  on-primary: '#ffffff'
  primary-container: '#131b2e'
  on-primary-container: '#7c839b'
  inverse-primary: '#bec6e0'
  secondary: '#515f74'
  on-secondary: '#ffffff'
  secondary-container: '#d5e3fd'
  on-secondary-container: '#57657b'
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
  secondary-fixed: '#d5e3fd'
  secondary-fixed-dim: '#b9c7e0'
  on-secondary-fixed: '#0d1c2f'
  on-secondary-fixed-variant: '#3a485c'
  tertiary-fixed: '#e0e3e5'
  tertiary-fixed-dim: '#c4c7c9'
  on-tertiary-fixed: '#191c1e'
  on-tertiary-fixed-variant: '#444749'
  background: '#fcf8fa'
  on-background: '#1b1b1d'
  surface-variant: '#e4e2e4'
typography:
  display-sm:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
    letterSpacing: -0.02em
  headline-sm:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '600'
    lineHeight: 24px
    letterSpacing: -0.01em
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
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
  label-xs:
    fontFamily: JetBrains Mono
    fontSize: 10px
    fontWeight: '500'
    lineHeight: 12px
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 12px
  lg: 16px
  xl: 24px
  gutter: 12px
  margin-mobile: 16px
  sidebar-width: 240px
---

## Brand & Style

The design system is built on the principles of **Operational Minimalism**. It is a utilitarian framework designed for high-density productivity where data clarity is the primary objective. The brand personality is calm, professional, and deterministic, favoring functional precision over decorative flair.

The UI avoids "marketing flourishes" such as large gradients, heavy shadows, or whimsical illustrations. Instead, it utilizes a structured, systematic approach to information architecture. The emotional response should be one of quiet focus and reliability—a tool that stays out of the way while providing maximum visibility into complex workflows.

## Colors

This design system employs a professional, cool-toned palette. The primary color is a deep Slate Blue, used for critical actions and navigational anchors to provide a sense of stability. 

The background hierarchy relies on subtle shifts in cool grays to differentiate surface areas without adding visual noise. 
- **Surface Primary:** Pure white (#FFFFFF) for content areas.
- **Surface Secondary:** Soft gray (#F8FAFC) for sidebars and inactive regions.
- **Accents:** High-contrast blue for interactive states.
- **Semantic Colors:** Success, Warning, and Error colors are used sparingly and with high saturation to ensure state changes are immediately recognizable against the neutral backdrop.

## Typography

Typography is the backbone of this design system. **Inter** is the primary typeface for its exceptional legibility at small sizes and its neutral, systematic character. To reinforce the utilitarian aesthetic, **JetBrains Mono** is introduced for metadata, timestamps, and status labels, providing a distinct visual "coding" for data points.

The hierarchy is tight. We prioritize small font sizes with generous line heights to maintain readability in high-density views. Letter spacing is slightly tightened for headings to maintain a compact, "buttoned-up" look.

## Layout & Spacing

The layout uses a **Fluid System with Fixed Sidebars**. The primary workspace expands to fill the viewport, while utility panels (sidebars/activity feeds) maintain fixed widths to ensure consistent tool access.

A **4px baseline grid** governs all spacing. In TaskBeacon Mini, "compact" is the default state. Margins and paddings are reduced to keep more data "above the fold."
- **Desktop:** 12-column grid within the fluid container; 12px gutters.
- **Density:** Components use `sm` (8px) or `md` (12px) padding as the standard internal spacing to achieve a dense but balanced feel.
- **Alignment:** All elements are strictly aligned to the grid to create a sense of order and deterministic logic.

## Elevation & Depth

This design system uses **Tonal Layers and Low-Contrast Outlines** rather than traditional shadows. Depth is conveyed through background color steps and 1px borders.

1.  **Level 0 (Base):** Primary background (#F8FAFC).
2.  **Level 1 (Cards/Panels):** Pure white (#FFFFFF) with a 1px border (#E2E8F0).
3.  **Level 2 (Popovers/Modals):** Pure white with a subtle, non-blurred 2px offset "block shadow" (#0F172A at 5% opacity) to provide a tactile sense of lift without softness.

This "Flat-Plus" approach ensures that the UI remains crisp and high-performance, avoiding the visual weight of heavy blurs.

## Shapes

The shape language is **Soft (0.25rem)**. This slight rounding takes the edge off the brutalist layout without making the UI feel overly consumer-focused or "bubbly."

- **Standard Elements:** 4px radius (Buttons, Inputs, Checkboxes).
- **Large Containers:** 8px radius (Cards, Modals).
- **Interactive States:** Focus rings should follow the 4px radius with a 2px offset to maintain clarity.

## Components

### Buttons
Buttons are strictly rectangular with 4px corners. 
- **Primary:** Deep Slate Blue background, white text. No gradient.
- **Secondary:** White background, 1px Slate border.
- **Ghost:** No border or background until hover; used for low-priority actions in dense lists.

### Task Cards
Cards are designed for information density. They feature a 1px Slate-200 border, no shadow, and internal padding of 12px. Labels (JetBrains Mono) are placed in the top-right for status, while the task title (Inter 14px Semi-bold) anchors the left.

### Form Fields
Inputs use a "contained" style with a 1px border. On focus, the border shifts to the Primary color with a 2px soft ring. Labels are always positioned above the input in `label-md` style for maximum clarity.

### Sidebars & Activity
The sidebar uses a slightly darker neutral background (#F1F5F9) to provide a clear anchor point for navigation. Activity feeds use a "timeline" aesthetic with 1px vertical connectors and `label-xs` timestamps.

### Status Chips
Small, high-contrast badges for "In Progress," "Done," or "Blocked." These use a light tint of the status color for the background and the full-saturation color for the text to ensure accessibility and immediate recognition.