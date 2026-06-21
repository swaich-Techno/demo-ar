---
name: B Socio AR Studio
colors:
  surface: '#11131c'
  surface-dim: '#11131c'
  surface-bright: '#373943'
  surface-container-lowest: '#0c0e17'
  surface-container-low: '#191b24'
  surface-container: '#1d1f29'
  surface-container-high: '#282933'
  surface-container-highest: '#32343e'
  on-surface: '#e1e1ef'
  on-surface-variant: '#d4c0d7'
  inverse-surface: '#e1e1ef'
  inverse-on-surface: '#2e303a'
  outline: '#9d8ba0'
  outline-variant: '#514255'
  surface-tint: '#ecb2ff'
  primary: '#ecb2ff'
  on-primary: '#520071'
  primary-container: '#bd00ff'
  on-primary-container: '#ffffff'
  inverse-primary: '#9900cf'
  secondary: '#d3fbff'
  on-secondary: '#00363a'
  secondary-container: '#00eefc'
  on-secondary-container: '#00686f'
  tertiary: '#ffaed9'
  on-tertiary: '#610046'
  tertiary-container: '#dd00a3'
  on-tertiary-container: '#fffeff'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#f8d8ff'
  primary-fixed-dim: '#ecb2ff'
  on-primary-fixed: '#320047'
  on-primary-fixed-variant: '#74009f'
  secondary-fixed: '#7df4ff'
  secondary-fixed-dim: '#00dbe9'
  on-secondary-fixed: '#002022'
  on-secondary-fixed-variant: '#004f54'
  tertiary-fixed: '#ffd8ea'
  tertiary-fixed-dim: '#ffaed9'
  on-tertiary-fixed: '#3c002a'
  on-tertiary-fixed-variant: '#890064'
  background: '#11131c'
  on-background: '#e1e1ef'
  surface-variant: '#32343e'
typography:
  display-lg:
    fontFamily: Space Grotesk
    fontSize: 72px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Space Grotesk
    fontSize: 40px
    fontWeight: '600'
    lineHeight: '1.2'
  headline-lg-mobile:
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
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-md:
    fontFamily: Geist
    fontSize: 14px
    fontWeight: '500'
    lineHeight: '1.2'
    letterSpacing: 0.05em
  label-sm:
    fontFamily: Geist
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1.2'
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 8px
  container-max: 1440px
  gutter: 24px
  margin-desktop: 64px
  margin-mobile: 20px
  stack-xs: 4px
  stack-md: 16px
  stack-xl: 48px
---

## Brand & Style
The design system is engineered for a cutting-edge AR creation environment. It embodies an **Innovative, Empowering, and Boundary-Pushing** personality. The aesthetic is rooted in a refined **Glassmorphic** style, utilizing depth, transparency, and light-emissions to simulate the layering of augmented reality interfaces.

The target audience consists of professional creators and tech-forward enthusiasts. The UI should evoke a sense of limitless creative potential, feeling like a high-performance "command center" for digital reality. Visuals are dominated by deep obsidian tones punctuated by vibrant neon light sources that serve as functional highlights.

## Colors
This design system utilizes a "Deep Space" palette to maximize the vibrance of AR assets. 

- **Primary (Electric Purple):** Used for main actions, active states, and primary brand moments.
- **Secondary (Cyan):** Used for technical information, data visualizations, and secondary interactions.
- **Tertiary (Magenta):** Used for creative tools, highlights, and specialized UI feedback.
- **Surface Strategy:** Surfaces are not solid; they use a layered approach of ultra-dark backgrounds and semi-transparent glass overlays with 40px background blurs.
- **Neon Glows:** Functional elements utilize subtle outer glows (box-shadows) in their respective brand colors to simulate emitted light.

## Typography
The typography system balances technical precision with high-impact editorial style. 

- **Headlines:** Space Grotesk provides a geometric, futuristic feel with its distinct "tech" character. It should be used for large displays and section headers.
- **Body:** Inter is used for all long-form content and tooltips to ensure maximum legibility against dark, blurred backgrounds.
- **Labels:** Geist (monospaced qualities) is utilized for UI controls, code snippets, and coordinate data (X, Y, Z axes), reinforcing the "studio" and "technical" nature of the platform.

## Layout & Spacing
The design system employs a **Fluid Grid** with generous white space to prevent the complex AR toolset from feeling cluttered. 

- **Desktop:** 12-column grid with 24px gutters. Content is typically housed in floating glass panels that adapt to viewport height.
- **Studio Workspace:** The central viewport (the "Stage") is expansive, with side panels (tools/properties) appearing as floating glass panes with 16px margins from the screen edge.
- **Responsive Behavior:** On smaller screens, side panels collapse into bottom sheets or drawer menus, prioritizing the visual canvas.

## Elevation & Depth
Depth is the core of this design system, achieved through **Glassmorphism** rather than traditional shadows.

- **Level 0 (Base):** Solid `#05060A` background.
- **Level 1 (Panels):** `rgba(255, 255, 255, 0.03)` with a `backdrop-filter: blur(40px)` and a 1px solid white border at 10% opacity.
- **Level 2 (Modals/Popovers):** Higher transparency `rgba(255, 255, 255, 0.06)` with a 1px border at 20% opacity and a faint outer glow matching the element's primary function (e.g., Cyan for info, Purple for action).
- **Interactions:** Elements should "lift" toward the user on hover by increasing the border opacity and the intensity of the background blur.

## Shapes
The shape language is **Modern and Balanced**. 

- **Panels & Cards:** Use a 1rem (16px) radius to soften the technical edge and feel more premium.
- **Buttons & Inputs:** Follow a 0.5rem (8px) radius for a precise, "machine-milled" look.
- **Active Indicators:** Use pill-shaped (full-round) geometry for status indicators and active toggles to differentiate them from structural layout elements.

## Components
- **Buttons:** Primary buttons are semi-transparent with a 1px neon border and a subtle "inner glow." On hover, they fill with a gradient of the brand color.
- **Glass Cards:** Used for AR asset previews. They must feature high-contrast image masking and thin white borders.
- **Input Fields:** Minimalist design—only a bottom border in the "inactive" state, transforming into a glowing neon frame when focused.
- **Chips/Tags:** Monospaced Geist font, small caps, with a background blur and a color-coded dot for categorization (e.g., #00F0FF for 'Script', #BD00FF for '3D Model').
- **Control Sliders:** Thin tracks with glowing "puck" handles that leave a trailing neon gradient as they move.
- **Hierarchy Navigation:** Breadcrumbs or tree-views for layer management should use thin "connector lines" to maintain the technical architectural feel.