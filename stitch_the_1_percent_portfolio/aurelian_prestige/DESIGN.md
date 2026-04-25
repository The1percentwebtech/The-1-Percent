---
name: Aurelian Prestige
colors:
  surface: '#16130b'
  surface-dim: '#16130b'
  surface-bright: '#3d392f'
  surface-container-lowest: '#110e07'
  surface-container-low: '#1f1b13'
  surface-container: '#231f17'
  surface-container-high: '#2d2a21'
  surface-container-highest: '#38342b'
  on-surface: '#eae1d4'
  on-surface-variant: '#d0c5af'
  inverse-surface: '#eae1d4'
  inverse-on-surface: '#343027'
  outline: '#99907c'
  outline-variant: '#4d4635'
  surface-tint: '#e9c349'
  primary: '#f2ca50'
  on-primary: '#3c2f00'
  primary-container: '#d4af37'
  on-primary-container: '#554300'
  inverse-primary: '#735c00'
  secondary: '#ffe2ab'
  on-secondary: '#402d00'
  secondary-container: '#ffbf00'
  on-secondary-container: '#6d5000'
  tertiary: '#bfcdff'
  on-tertiary: '#082b72'
  tertiary-container: '#97b0ff'
  on-tertiary-container: '#254188'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#ffe088'
  primary-fixed-dim: '#e9c349'
  on-primary-fixed: '#241a00'
  on-primary-fixed-variant: '#574500'
  secondary-fixed: '#ffdfa0'
  secondary-fixed-dim: '#fbbc00'
  on-secondary-fixed: '#261a00'
  on-secondary-fixed-variant: '#5c4300'
  tertiary-fixed: '#dbe1ff'
  tertiary-fixed-dim: '#b4c5ff'
  on-tertiary-fixed: '#00174b'
  on-tertiary-fixed-variant: '#27438a'
  background: '#16130b'
  on-background: '#eae1d4'
  surface-variant: '#38342b'
typography:
  display-xl:
    fontFamily: Noto Serif
    fontSize: 80px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Noto Serif
    fontSize: 48px
    fontWeight: '600'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Noto Serif
    fontSize: 32px
    fontWeight: '500'
    lineHeight: '1.3'
  body-lg:
    fontFamily: Manrope
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Manrope
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-sm:
    fontFamily: Manrope
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1'
    letterSpacing: 0.05em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 8px
  xs: 4px
  sm: 12px
  md: 24px
  lg: 48px
  xl: 80px
  container-max: 1280px
  gutter: 32px
---

## Brand & Style

This design system embodies a philosophy of "Accessible Excellence." It balances the exclusivity of a high-end investment or luxury brand with a warm, growth-oriented friendliness. The aesthetic is rooted in **Minimalism** to ensure clarity and focus, layered with **Glassmorphism** and **Light-driven Depth** to create a sense of modernity and digital tactility.

The emotional response should be one of aspiration and belonging. Users should feel they are entering an elite space that is nonetheless welcoming and designed for their personal expansion. Visuals are anchored by deep, infinite obsidian surfaces, contrasted against kinetic, organic light effects that mimic a living pulse.

## Colors

The palette is strictly dark-mode by default to emphasize the "Obsidian" depth. 

- **Surfaces:** Use Neutral-950 (#0A0A0A) as the base canvas. Secondary surfaces (cards, modals) should use a slightly elevated Neutral-900 with low-opacity gold strokes.
- **Highlights:** Gold (#D4AF37) is reserved for primary actions, branding, and critical focus states. Amber (#FFBF00) serves as a kinetic accent, used for "growth" indicators and pulsating interactive cues.
- **Atmospheric Light:** Implement subtle radial gradients of Amber and Gold in the background (0-5% opacity) to prevent the dark interface from feeling flat or sterile.

## Typography

This design system uses a high-contrast typographic pairing to signal both heritage and innovation.

- **Headings:** `notoSerif` provides a timeless, literary quality. In the logo and major display headers, the numeral '1' should be scaled to 120-140% of the surrounding text height to create a distinct visual anchor.
- **Body:** `manrope` offers a clean, technical, yet friendly contrast. Its geometric clarity ensures readability against dark backgrounds.
- **Formatting:** Use generous line heights for body text to maintain an "approachable" and "breezy" reading experience despite the heavy color palette.

## Layout & Spacing

The layout follows a **Fixed Grid** model centered on the screen to evoke the feel of a curated gallery or premium editorial. 

- **Grid:** A 12-column system with wide 32px gutters to allow elements plenty of "room to breathe."
- **Margins:** Use large outer margins (Section XL) to pull focus toward the center of the viewport.
- **Rhythm:** Spacing should be used aggressively to separate content blocks, ensuring that the "Elite" brand personality is felt through intentional whitespace.

## Elevation & Depth

Depth is conveyed through light and transparency rather than traditional heavy shadows.

- **Tonal Layers:** Higher-level elements (like cards) use a 5% white overlay on the obsidian base to appear closer to the user.
- **Light Effects:** Instead of drop shadows, use "Bloom Shadows"—subtle, pulsating outer glows in Gold (#D4AF37) with high blur (40px+) and low opacity (10-15%).
- **Glassmorphism:** Modals and navigation bars should use a backdrop blur (20px) with a semi-transparent Obsidian fill (80% opacity) and a 1px Gold border at 10% opacity.

## Shapes

The shape language is sophisticated and "soft-modern."

- **Corner Radii:** A base radius of 0.5rem (8px) is used for standard components, while large containers and cards use 1.5rem (24px) to feel more inviting and less aggressive.
- **Interactive Elements:** Buttons and tags should utilize a slightly more rounded profile (up to full pill-shape for chips) to reinforce the "friendly" aspect of the brand.

## Components

### Custom Cursor
A 24px circular "Orb" cursor. It should have a 2px Gold border and a center Amber glow. It "pulsates" (scales between 0.8x and 1.2x) every 2 seconds. On hover over interactables, it should expand to 64px and become a translucent Gold blur.

### Interactive Cards
Cards use a subtle 1px border (#D4AF37 at 10% opacity). On hover, apply a `transform: scale(1.02) translateY(-4px)` with a "pop" easing function (`cubic-bezier(0.34, 1.56, 0.64, 1)`). The border opacity should increase to 50% during hover.

### Buttons
Primary buttons feature a Gold-to-Amber linear gradient (45 degrees). They must include a subtle "inner glow" and a pulsating light effect on the text itself during hover states to signify "energy" and "growth."

### Pulsating Light Elements
Strategic decorative elements (dots, thin lines, or background orbs) should have a slow CSS keyframe animation mimicking a heartbeat, cycling the opacity of an Amber glow.

### Inputs & Forms
Form fields are bottom-border only (Gold, 1px) to maintain a minimalist profile. Upon focus, the border should animate into a full-ring Gold glow.