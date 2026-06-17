---
name: Luminous Trade System
colors:
  surface: '#081519'
  surface-dim: '#081519'
  surface-bright: '#2e3b3f'
  surface-container-lowest: '#041014'
  surface-container-low: '#101d21'
  surface-container: '#142225'
  surface-container-high: '#1f2c30'
  surface-container-highest: '#2a373b'
  on-surface: '#d7e5ea'
  on-surface-variant: '#bfc8cb'
  inverse-surface: '#d7e5ea'
  inverse-on-surface: '#253237'
  outline: '#8a9295'
  outline-variant: '#40484b'
  surface-tint: '#94d0e1'
  primary: '#96d2e3'
  on-primary: '#003641'
  primary-container: '#7bb6c7'
  on-primary-container: '#004855'
  inverse-primary: '#276675'
  secondary: '#ffb4a6'
  on-secondary: '#630f04'
  secondary-container: '#862919'
  on-secondary-container: '#ff9f8d'
  tertiary: '#fcbb8b'
  on-tertiary: '#4d2603'
  tertiary-container: '#dea072'
  on-tertiary-container: '#613611'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#b0ecfe'
  primary-fixed-dim: '#94d0e1'
  on-primary-fixed: '#001f26'
  on-primary-fixed-variant: '#004e5d'
  secondary-fixed: '#ffdad3'
  secondary-fixed-dim: '#ffb4a6'
  on-secondary-fixed: '#3f0300'
  on-secondary-fixed-variant: '#822617'
  tertiary-fixed: '#ffdcc4'
  tertiary-fixed-dim: '#fab989'
  on-tertiary-fixed: '#301400'
  on-tertiary-fixed-variant: '#683c16'
  background: '#081519'
  on-background: '#d7e5ea'
  surface-variant: '#2a373b'
typography:
  display-lg:
    fontFamily: Hanken Grotesk
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Hanken Grotesk
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
  headline-md:
    fontFamily: Hanken Grotesk
    fontSize: 24px
    fontWeight: '500'
    lineHeight: 32px
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-md:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
    letterSpacing: 0.05em
  label-sm:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
    letterSpacing: 0.05em
  headline-lg-mobile:
    fontFamily: Hanken Grotesk
    fontSize: 28px
    fontWeight: '600'
    lineHeight: 36px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 4px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 40px
  container-max: 1440px
---

## Brand & Style

This design system is engineered for professional traders who require high-density data visualization without the cognitive load typically associated with financial tools. The brand personality is **sophisticated, precise, and fluid**, prioritizing clarity through a synthesis of **Minimalism** and **Glassmorphism**.

The visual narrative centers on "Translucent Precision." By blending the structured hierarchy of Material You with the ethereal depth of Apple-inspired glass effects, the UI feels both grounded and modern. The emotional response should be one of calm focus—transforming complex calculations into a tactile, manageable experience. 

Key stylistic pillars include:
- **Depth through Refraction:** Using backdrop blurs to maintain context while isolating active tasks.
- **Organic Motion:** Interactive elements should feel liquid and responsive, particularly in data transitions.
- **Intentional Negative Space:** Generous breathing room around data points to prevent "information drowning."

## Colors

The design system utilizes a dual-thematic approach optimized for different trading environments. While the default mode is **Dark**, the system maintains a consistent logical mapping for Light mode.

- **Primary (Dark):** #7BB6C7 (Soft Cyan). Used for growth indicators, primary actions, and "liquid" highlights.
- **Primary (Light):** #B54B38 (Deep Terracotta). Used for urgency, primary CTA focal points, and warm data visualizations.
- **Surface Strategy:** Surfaces are not solid. They utilize a `backdrop-filter: blur(16px)` combined with a semi-transparent hex color (60% in dark, 70% in light) to allow background gradients or underlying data to softly peak through.
- **Functional Accents:** Success and error states should lean into the primary colors of the opposing mode to create a sophisticated, non-standard palette (e.g., Soft Cyan for "Gain", Deep Terracotta for "Loss").

## Typography

The typographic scale emphasizes high legibility and technical rigor. 

- **Hanken Grotesk** is used for headlines to provide a sharp, contemporary edge that feels "engineered."
- **Inter** handles the bulk of body copy and interface elements, ensuring neutral readability across various screen densities.
- **JetBrains Mono** is reserved for all numerical data, trade IDs, and tickers. Its monospaced nature ensures that fluctuating numbers don't cause layout jumps and are easily scannable in tabular formats.

Use **Purposeful Weight Contrast** to guide the eye: Large, light-weight numbers for primary balances, paired with small, bold JetBrains Mono labels for secondary metrics.

## Layout & Spacing

The design system employs a **Fluid-Fixed Hybrid Grid**. The sidebar and utility panels occupy fixed widths, while the primary "Calculation Canvas" expands to fill available space.

- **Grid Model:** A 12-column grid for desktop with 24px gutters. On mobile, this collapses to a 4-column grid with 16px margins.
- **Spacing Rhythm:** Based on a 4px baseline. Components use 16px (4 units) or 24px (6 units) of internal padding to maintain a sense of airiness.
- **Data Density:** In complex trade views, vertical spacing between rows can be reduced to 8px, but horizontal "breathability" must be maintained at 24px.
- **Mobile Reflow:** Complex calculators should use a vertically stacked card approach, where each "Glass Layer" becomes a full-width container.

## Elevation & Depth

Hierarchy is established through **Tonal Stacking** and **Refractive Layers** rather than heavy shadows.

- **Level 0 (Background):** Solid `#0E1517` (Dark) or `#F8F9FA` (Light).
- **Level 1 (Main Panels):** 60% opacity with 16px backdrop-blur. Features a subtle 1px inner border (white at 10% opacity) to catch "light" at the edges.
- **Level 2 (Active Modals/Popovers):** Higher opacity (80%) and a soft, diffused shadow (`0 12px 40px rgba(0,0,0,0.3)`). 
- **The "Glow" Effect:** Active states or critical alerts utilize an outer glow using the Primary color with a 20px blur and low opacity (20%) to simulate light emanating from beneath the glass.

## Shapes

The shape language is consistently **Rounded**. Sharp corners are avoided to reinforce the "liquid" and approachable nature of the system.

- **Standard Containers:** 16px (1rem) corner radius.
- **Large Sections/Cards:** 24px (1.5rem) corner radius.
- **Small Elements (Buttons, Inputs):** 12px (0.75rem) corner radius.
- **Liquid Visuals:** The "Profit Distribution Bar" should have fully rounded (pill-shaped) ends. 

All interactive surfaces should utilize a 1px "stroke" that acts as a glass edge, providing definition against the blurred background.

## Components

### Buttons
- **Primary:** Gradient-filled (Primary color to a slightly lighter tint), 12px radius. On hover, the "inner glow" intensifies.
- **Glass Action:** Transparent background, 1px border, heavy backdrop-blur. Used for secondary dashboard actions.

### Input Fields
- **Calculation Inputs:** Minimalist underline or soft-glass background. Numerical values appear in JetBrains Mono. Focus state triggers a subtle primary color glow.

### The "Glowing Liquid" Bar
- A custom component for profit distribution. Each segment is a distinct color with a `filter: blur(2px)` and a CSS animation simulating a sine wave movement at the segment junctions. Transitions between values should be "spring" based and fluid.

### Trade Cards
- Glass panels with 16px radius. Contain condensed data with `label-sm` headers. Active dragging states should increase the backdrop-blur and scale the card to 102% to simulate the element "lifting" off the glass surface.

### Chips/Badges
- Pill-shaped with low-opacity fills of the Primary colors. Used for status (e.g., "Long", "Short", "Pending").