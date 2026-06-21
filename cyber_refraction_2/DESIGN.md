---
name: Cyber-Refraction
colors:
  surface: '#051424'
  surface-dim: '#051424'
  surface-bright: '#2c3a4c'
  surface-container-lowest: '#010f1f'
  surface-container-low: '#0d1c2d'
  surface-container: '#122131'
  surface-container-high: '#1c2b3c'
  surface-container-highest: '#273647'
  on-surface: '#d4e4fa'
  on-surface-variant: '#b9cacb'
  inverse-surface: '#d4e4fa'
  inverse-on-surface: '#233143'
  outline: '#849495'
  outline-variant: '#3b494b'
  surface-tint: '#00dbe8'
  primary: '#d3fbff'
  on-primary: '#00363a'
  primary-container: '#00eefc'
  on-primary-container: '#00686e'
  inverse-primary: '#006970'
  secondary: '#ecb2ff'
  on-secondary: '#520071'
  secondary-container: '#cf5cff'
  on-secondary-container: '#480063'
  tertiary: '#f3f2ff'
  on-tertiary: '#2e303a'
  tertiary-container: '#d6d6e3'
  on-tertiary-container: '#5b5d68'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#79f4ff'
  primary-fixed-dim: '#00dbe8'
  on-primary-fixed: '#002022'
  on-primary-fixed-variant: '#004f54'
  secondary-fixed: '#f8d8ff'
  secondary-fixed-dim: '#ecb2ff'
  on-secondary-fixed: '#320047'
  on-secondary-fixed-variant: '#74009f'
  tertiary-fixed: '#e1e1ef'
  tertiary-fixed-dim: '#c5c5d2'
  on-tertiary-fixed: '#191b24'
  on-tertiary-fixed-variant: '#454651'
  background: '#051424'
  on-background: '#d4e4fa'
  surface-variant: '#273647'
typography:
  display-lg:
    fontFamily: Space Grotesk
    fontSize: 72px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.04em
  headline-xl:
    fontFamily: Space Grotesk
    fontSize: 48px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  headline-xl-mobile:
    fontFamily: Space Grotesk
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Space Grotesk
    fontSize: 24px
    fontWeight: '500'
    lineHeight: '1.3'
  body-lg:
    fontFamily: Space Grotesk
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Space Grotesk
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.5'
  label-sm:
    fontFamily: Space Grotesk
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1.0'
    letterSpacing: 0.05em
spacing:
  unit: 4px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 64px
  container-max: 1440px
---

## Brand & Style
The brand personality is authoritative, technical, and forward-looking, designed to instill confidence in enterprise stakeholders. The "Cyber-Refraction" aesthetic blends the precision of high-end developer tools with the visual depth of modern AR/VR interfaces.

The design style utilizes a **High-Contrast / Modern** approach with subtle **Glassmorphism**. It emphasizes sharp edges, dark surfaces, and luminous accents that suggest a high-fidelity digital environment. The emotional goal is to feel premium and "next-gen," moving away from playful consumer vibes toward a focused, professional workspace.

## Colors
The palette is rooted in a deep, monochromatic base to ensure enterprise-grade stability, with high-energy accents used for interactive elements and data visualization.

- **Foundational Surface:** Deep Slate (#11131c) serves as the primary background, providing a rich, low-strain canvas.
- **Action Cyan:** High-Contrast Cyan (#00eefc) is used for primary actions, success states, and technical highlights.
- **Structural Purple:** Purple (#bd00ff) is reserved for secondary navigation, branding elements, and decorative refraction effects.
- **Functional Grays:** A range of cool grays are used for secondary text and subtle borders to maintain hierarchy without clutter.

## Typography
Space Grotesk is the sole typeface, utilized for its technical, geometric character and high legibility in dark environments. 

- **Display & Headlines:** Use tight letter spacing and bold weights to create an impactful, editorial feel for sales decks.
- **Body Text:** Use regular weights with generous line height to ensure readability of technical specifications.
- **Labels:** Small labels should always be uppercase with increased letter spacing to mimic technical blueprints or HUD interfaces.

## Layout & Spacing
The layout follows a **Fixed Grid** model for the desktop sales deck experience to ensure pixel-perfect presentation, transitioning to a fluid model for mobile viewing.

- **Grid:** A 12-column grid is used for desktop with 24px gutters. Elements should align strictly to the grid to reinforce the "technical" nature of the design.
- **Rhythm:** All spacing is based on a 4px baseline unit. 
- **Adaptation:** On mobile, margins reduce to 16px and the 12-column layout collapses to a single-column stack. Heavy use of vertical padding (80px+) between sections is encouraged to maintain a premium, airy feel.

## Elevation & Depth
In this design system, depth is communicated through light refraction rather than traditional shadows.

- **Tonal Layers:** Objects closer to the user are lighter shades of slate or semi-transparent glass.
- **Refraction:** Use 1px "inner-glow" borders in Cyan or Purple on the top and left edges of cards to simulate a light source hitting a glass edge.
- **Backdrop Blurs:** High-elevation components (modals, dropdowns) should use a `blur(20px)` effect with a 40% opaque slate background.
- **Glows:** Primary buttons and active states feature a soft, outer glow (0px 0px 15px) matching their accent color to suggest luminosity.

## Shapes
The shape language is **Sharp**. Elements utilize 0px border radii to emphasize precision and a "pro-tool" aesthetic. 

Small exceptions are made for strictly "organic" data points in charts, but all containers, buttons, and input fields must maintain 90-degree corners. This rigidity creates the "Cyber" structure necessary for the design system's narrative.

## Components
- **Buttons:** Primary buttons are solid Cyan with black text. Secondary buttons are Ghost-style with a 1px Cyan border. All buttons have 0px radius and a hover state that increases the outer glow intensity.
- **Input Fields:** Deep slate background with a 1px bottom border only (Cyan). Labels sit above the field in `label-sm` style.
- **Cards:** Background is a slightly lighter slate than the base. Cards must feature a 1px Cyan or Purple top-border to denote category or hierarchy.
- **Chips:** Small, sharp-edged rectangles. Active chips are filled Purple; inactive chips are outlined in Gray.
- **Data Visualization:** Use high-contrast lines. Area charts should use a gradient fill from Cyan (100% opacity) to Transparent (0% opacity) to mimic a digital readout.
- **AR Viewports:** Frames for AR content should have "corner bracket" icons in Cyan to simulate a camera viewfinder.