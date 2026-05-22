---
name: Cyber Shredder
colors:
  surface: '#131314'
  surface-dim: '#131314'
  surface-bright: '#3a393a'
  surface-container-lowest: '#0e0e0f'
  surface-container-low: '#1c1b1c'
  surface-container: '#201f20'
  surface-container-high: '#2a2a2b'
  surface-container-highest: '#353436'
  on-surface: '#e5e2e3'
  on-surface-variant: '#baccb0'
  inverse-surface: '#e5e2e3'
  inverse-on-surface: '#313031'
  outline: '#85967c'
  outline-variant: '#3c4b35'
  surface-tint: '#2ae500'
  primary: '#efffe3'
  on-primary: '#053900'
  primary-container: '#39ff14'
  on-primary-container: '#107100'
  inverse-primary: '#106e00'
  secondary: '#ffb59c'
  on-secondary: '#5c1900'
  secondary-container: '#fa5c1c'
  on-secondary-container: '#511500'
  tertiary: '#ecfdff'
  on-tertiary: '#00363a'
  tertiary-container: '#55f2ff'
  on-tertiary-container: '#006c73'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#79ff5b'
  primary-fixed-dim: '#2ae500'
  on-primary-fixed: '#022100'
  on-primary-fixed-variant: '#095300'
  secondary-fixed: '#ffdbcf'
  secondary-fixed-dim: '#ffb59c'
  on-secondary-fixed: '#390c00'
  on-secondary-fixed-variant: '#832700'
  tertiary-fixed: '#7df4ff'
  tertiary-fixed-dim: '#00dbe9'
  on-tertiary-fixed: '#002022'
  on-tertiary-fixed-variant: '#004f54'
  background: '#131314'
  on-background: '#e5e2e3'
  surface-variant: '#353436'
  surface-void: '#0A0A0B'
  neon-aurora: '#39FF14'
  passion-orange: '#FF5F1F'
  cyber-cyan: '#00F0FF'
  glass-stroke: rgba(255, 255, 255, 0.12)
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
    fontWeight: '700'
    lineHeight: 40px
  headline-lg-mobile:
    fontFamily: Space Grotesk
    fontSize: 24px
    fontWeight: '700'
    lineHeight: 32px
  body-md:
    fontFamily: Hanken Grotesk
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-tech:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
    letterSpacing: 0.05em
  numeral-xl:
    fontFamily: Space Grotesk
    fontSize: 64px
    fontWeight: '700'
    lineHeight: 64px
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 4px
  gutter: 16px
  margin-mobile: 20px
  margin-desktop: 64px
  slice-reveal: 25%
---

## Brand & Style

The design system embodies a "Cyberpunk-Street" hybrid, merging the raw, rebellious energy of skateboard culture with a high-tech digital aesthetic. It targets a young, tech-savvy audience, evoking feelings of high-octane energy, futuristic innovation, and urban grit.

The visual style is a blend of **High-Contrast Bold** and **Cyberpunk**. It utilizes heavy dark backgrounds to allow neon accents to "pop," simulating a midnight skate session in a neon-lit metropolis. A global film grain/noise texture is applied to all surfaces to provide a cinematic, tactile quality that bridges the gap between digital interfaces and physical street textures. 

Key motifs include:
- **Kinetic Energy:** Use of diagonal lines and "slice" reveals to imply motion.
- **Tech-Literalism:** Visible container guide lines and decorative numbering that mimic heads-up displays (HUDs) or technical blueprints.
- **Street Grit:** Subtle noise overlays and bold, impactful typography that feels like digital graffiti.

## Colors

The palette is optimized for a dark-mode-first experience. The base is a deep, near-black **Surface-Void** (#0A0A0B) which serves as the canvas for high-chroma neon accents. 

- **Primary (Neon Aurora):** Used for primary actions, success states, and key decorative "circuitry" lines.
- **Secondary (Passionate Orange):** Reserved for high-energy call-outs, warnings, or interactive highlights that need to contrast against the green.
- **Tertiary (Cyber Cyan):** Used for secondary technical data, info-labels, and subtle glow effects.
- **Neutral:** A range of deep grays derived from the base hex, used for secondary surfaces and container borders.

A global **Grain Texture** should be overlaid at 3-5% opacity across all color fills to maintain the cinematic grit.

## Typography

The typography system prioritizes a "tech-centric" feel. 
- **Headlines:** Use **Space Grotesk** for its geometric, futuristic personality. Headlines should often be uppercase or use tight letter spacing for a more aggressive, condensed "poster" feel.
- **Body:** **Hanken Grotesk** provides a clean, contemporary sans-serif experience that remains highly legible against dark backgrounds.
- **Data & Numbers:** **JetBrains Mono** is used for decorative numbering, technical metadata, and UI labels, reinforcing the "coding" aspect of the brand.

**Decorative Numbering:** Large, low-opacity background numerals (e.g., "01", "02") should be used to anchor sections, acting as both a navigational aid and a design element.

## Layout & Spacing

This design system utilizes a **Fixed Grid** with an emphasis on **4-column slice reveals**. 

- **The Slice Model:** For hero sections or feature reveals, the screen is split into four vertical "slices." Content can enter via vertical slide animations within these slices.
- **Vertical Guides:** Thin, 1px lines (using `glass-stroke`) should run vertically across the background, aligned to the grid gutters, to create a "technical drawing" appearance.
- **Margins:** Desktop layouts use generous 64px margins to allow the "tech" decorative elements (lines, numbers) to breathe. Mobile scales down to a compact 20px margin.
- **Rhythm:** All spacing (padding, gaps) must be multiples of the 4px base unit to ensure mathematical precision.

## Elevation & Depth

Hierarchy is established through **Glassmorphism** and **Tonal Layering** rather than traditional drop shadows.

1.  **Base Layer:** The grain-textured #0A0A0B surface.
2.  **Glass Layer:** Semi-transparent surfaces (15-25% opacity) with a 20px backdrop blur. These layers use a 1px `glass-stroke` border to define their edges.
3.  **Neon Glow:** Elements of high importance (active buttons, lightning icons) utilize a subtle outer glow (0px blur 8px spread) in their respective accent color to simulate light emission.
4.  **Z-Index Logic:** Visual depth is created by stacking "glass" cards over the vertical background guide lines, allowing the lines to be partially visible through the blur.

## Shapes

The shape language is **Soft (0.25rem)**. While the overall vibe is aggressive and tech-heavy, micro-rounded corners prevent the UI from feeling dated or overly "brutalist."

- **Containers:** 4px (0.25rem) radius.
- **Interactive Elements:** 8px (0.5rem) radius for buttons and input fields to make them distinct from structural containers.
- **Decorative Lines:** These should remain sharp or capped with 45-degree angled "snipped" corners to mimic circuit board traces.

## Components

- **Buttons:** High-contrast fills using Neon Aurora or Passionate Orange. Text should be black (#000000) for maximum legibility on bright backgrounds. Use a "glow" state on hover.
- **Cards:** Glassmorphic containers with 1px borders. Include a decorative "0X" number in the top-right corner using JetBrains Mono.
- **Chips:** Small, outlined elements using the accent color with a subtle 10% opacity background fill.
- **Input Fields:** Dark background (#000000) with a `glass-stroke` border that transitions to `neon-aurora` on focus.
- **Icons:** Use **Solar** or **Lucide** sets. Icons should be styled with a thin stroke. Important icons (lightning, chips) can carry a subtle glow.
- **Container Guides:** Include non-functional, decorative "corner brackets" on major UI sections to reinforce the technical HUD aesthetic.