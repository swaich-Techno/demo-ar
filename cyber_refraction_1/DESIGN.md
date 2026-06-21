---
name: Cyber-Refraction
colors:
  surface: '#11131c'
  surface-dim: '#11131c'
  surface-bright: '#373943'
  surface-container-lowest: '#0c0e17'
  surface-container-low: '#191b25'
  surface-container: '#1d1f29'
  surface-container-high: '#282933'
  surface-container-highest: '#32343e'
  on-surface: '#e1e1ef'
  on-surface-variant: '#b9cacb'
  inverse-surface: '#e1e1ef'
  inverse-on-surface: '#2e303a'
  outline: '#849495'
  outline-variant: '#3b494b'
  surface-tint: '#00dbe8'
  primary: '#d3fbff'
  on-primary: '#00363a'
  primary-container: '#00eefc'
  on-primary-container: '#00686e'
  inverse-primary: '#006970'
  secondary: '#c2c5de'
  on-secondary: '#2b2f43'
  secondary-container: '#44485d'
  on-secondary-container: '#b4b7d0'
  tertiary: '#f9f1ff'
  on-tertiary: '#3c0090'
  tertiary-container: '#e0d0ff'
  on-tertiary-container: '#710cff'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#79f4ff'
  primary-fixed-dim: '#00dbe8'
  on-primary-fixed: '#002022'
  on-primary-fixed-variant: '#004f54'
  secondary-fixed: '#dee1fb'
  secondary-fixed-dim: '#c2c5de'
  on-secondary-fixed: '#161b2d'
  on-secondary-fixed-variant: '#42465a'
  tertiary-fixed: '#e9ddff'
  tertiary-fixed-dim: '#d1bcff'
  on-tertiary-fixed: '#23005b'
  on-tertiary-fixed-variant: '#5700c9'
  background: '#11131c'
  on-background: '#e1e1ef'
  surface-variant: '#32343e'
  glass-stroke: rgba(255, 255, 255, 0.1)
  neon-glow: rgba(0, 238, 252, 0.4)
  surface-overlay: rgba(255, 255, 255, 0.03)
typography:
  display-lg:
    fontFamily: Space Grotesk
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Space Grotesk
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
  headline-lg-mobile:
    fontFamily: Space Grotesk
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  body-md:
    fontFamily: Space Grotesk
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
    letterSpacing: 0.1em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 4px
  gutter: 24px
  margin-desktop: 64px
  margin-mobile: 20px
  container-max: 1440px
---

## Brand & Style
This design system is built for a high-tech, augmented reality studio environment. The personality is futuristic, technical, and immersive, evoking the feeling of a digital cockpit or an advanced HUD (Heads-Up Display).

The design style is **Glassmorphism mixed with High-Contrast Cyberpunk**. It utilizes deep, dark surfaces as a canvas for vibrant, glowing accents. Elements should feel like they are floating in a 3D space, using translucent layers, background blurs, and sharp, geometric lines to maintain a professional yet cutting-edge aesthetic.

## Colors
The palette is dominated by the "Void" background—a deep navy that provides the necessary contrast for the "Pulse" teal accent.

- **Primary (Pulse Teal):** Used for interactive states, primary actions, and critical data highlights. It should often be accompanied by a subtle outer glow.
- **Neutral (Void):** The foundation of the UI. All surfaces are derived from this base, moving toward lighter navy shades for higher elevation.
- **Secondary (Obsidian):** Used for card backgrounds and container surfaces.
- **Tertiary (Ion Purple):** A secondary accent used for supplementary data visualizations or alternate category states to prevent the UI from feeling monochromatic.

## Typography
We use **Space Grotesk** as the primary typeface for its geometric, technical character that feels inherently digital. For technical data and UI labels, we introduce **JetBrains Mono** to reinforce the developer-centric, AR studio vibe.

All headlines should use tighter letter spacing to maintain a "locked-in" architectural look. Labels and captions should be set in uppercase with increased letter spacing to ensure legibility against dark, blurred backgrounds.

## Layout & Spacing
The design system follows a **12-column fluid grid** for desktop and a **4-column grid** for mobile. The spacing rhythm is strictly based on a **4px baseline**, ensuring that even small technical components feel aligned and intentional.

Layouts should favor ample "breathing room" around glass panels to allow the background blurs to be effective. Content is often organized into "Modules"—contained units that can be rearranged dynamically, mimicking the interface of an AR creation tool.

## Elevation & Depth
Depth is created through transparency and "Stacking" rather than traditional shadows.

1.  **Backdrop Blur:** All elevated panels must use a `backdrop-filter: blur(12px)`.
2.  **Inner Glow/Stroke:** Use a 1px semi-transparent white top-border or full border to define the edge of glass elements.
3.  **Luminance:** Higher elevation is represented by increased opacity of the white overlay (e.g., 3% for base cards, 8% for modals).
4.  **Shadows:** When used, shadows should be highly diffused and tinted with the primary teal color at very low opacity (5-10%) to suggest light emitting from the element.

## Shapes
The shape language is "Soft-Technical." We avoid fully organic circles in favor of small, precise radii that suggest precision engineering. 

- **Containers:** Use `rounded-sm` (4px) for most UI cards and buttons.
- **Accents:** Use 45-degree chamfered corners (clipped corners) sparingly for decorative "frame" elements to push the futuristic aesthetic.

## Components

- **Buttons:** Primary buttons use a solid Teal fill with black text. Secondary buttons use a "Ghost" style with a teal border and backdrop blur.
- **Glass Cards:** The signature component. Features a subtle border (`glass-stroke`), a dark translucent fill, and a high-intensity backdrop blur.
- **Inputs:** Fields should have a dark, recessed look with a 1px bottom border that "lights up" in teal when focused.
- **Chips/Badges:** Use JetBrains Mono for text. These should look like small LED readouts, with low-opacity teal backgrounds.
- **Progress Indicators:** Use thin, glowing lines without rounded end-caps to maintain the technical, geometric feel.
- **Studio-Specific Components:** Include "Viewport Overlays," "Coordinate Pickers," and "Layer Lists" that utilize high-density layouts and monospaced typography.