---
name: Midnight Laboratory
colors:
  surface: '#0c1609'
  surface-dim: '#0c1609'
  surface-bright: '#323c2d'
  surface-container-lowest: '#071105'
  surface-container-low: '#141e11'
  surface-container: '#182214'
  surface-container-high: '#222d1e'
  surface-container-highest: '#2d3828'
  on-surface: '#dae6d0'
  on-surface-variant: '#baccb0'
  inverse-surface: '#dae6d0'
  inverse-on-surface: '#293324'
  outline: '#85967c'
  outline-variant: '#3c4b35'
  surface-tint: '#2ae500'
  primary: '#efffe3'
  on-primary: '#053900'
  primary-container: '#39ff14'
  on-primary-container: '#107100'
  inverse-primary: '#106e00'
  secondary: '#d3fbff'
  on-secondary: '#00363a'
  secondary-container: '#00eefc'
  on-secondary-container: '#00686f'
  tertiary: '#fff8f7'
  on-tertiary: '#442927'
  tertiary-container: '#ffd3ce'
  on-tertiary-container: '#7a5955'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#79ff5b'
  primary-fixed-dim: '#2ae500'
  on-primary-fixed: '#022100'
  on-primary-fixed-variant: '#095300'
  secondary-fixed: '#7df4ff'
  secondary-fixed-dim: '#00dbe9'
  on-secondary-fixed: '#002022'
  on-secondary-fixed-variant: '#004f54'
  tertiary-fixed: '#ffdad6'
  tertiary-fixed-dim: '#e7bdb8'
  on-tertiary-fixed: '#2c1513'
  on-tertiary-fixed-variant: '#5d3f3c'
  background: '#0c1609'
  on-background: '#dae6d0'
  surface-variant: '#2d3828'
typography:
  h1:
    fontFamily: Space Grotesk
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  h2:
    fontFamily: Space Grotesk
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: -0.01em
  h3:
    fontFamily: Space Grotesk
    fontSize: 24px
    fontWeight: '500'
    lineHeight: '1.3'
    letterSpacing: 0em
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
    letterSpacing: 0em
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.5'
    letterSpacing: 0em
  code-sm:
    fontFamily: Space Grotesk
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1.5'
    letterSpacing: 0.05em
  label-caps:
    fontFamily: Space Grotesk
    fontSize: 12px
    fontWeight: '700'
    lineHeight: '1'
    letterSpacing: 0.1em
spacing:
  unit: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 40px
  grid-gutter: 20px
  container-max: 1440px
---

## Brand & Style

The design system is engineered for the high-intensity environment of an electronics maker space. The brand personality is clinical, technical, and forward-looking, evoking the feeling of a sophisticated Heads-Up Display (HUD) used in a high-tech research facility. 

The aesthetic blends **Futuristic Minimalism** with **Cybernetic Brutalism**. It prioritizes data density and functional clarity while utilizing "active" visual elements like circuit traces and glowing indicators to signal power and connectivity. The emotional response is one of precision, expertise, and immersion in a digital-physical hybrid workspace.

## Colors

The palette is strictly dark-mode, anchored by a "Void Black" base (#0A0A0A) for the deepest layers and "Charcoal Surface" (#121212) for UI containers. 

The primary accent is "Neon Kinetic Green" (#39FF14), used exclusively for active states, successful connections, and primary calls to action. A secondary "Cyan Glitch" (#00F0FF) is utilized for data visualization highlights and informational alerts. Whites and grays are kept cool-toned to maintain the technical, "cold" atmosphere of a laboratory.

## Typography

This design system uses **Space Grotesk** for headings and technical data to provide a sharp, geometric, and futuristic feel. Its unique letterforms reinforce the "laboratory" aesthetic. For long-form reading and standard UI labels, **Inter** provides high legibility and a systematic, utilitarian structure.

All labels for hardware pins, sensor data, and terminal outputs should be rendered in **Space Grotesk** with increased letter spacing and uppercase styling to mimic industrial equipment markings.

## Layout & Spacing

The layout follows a **Fixed-Grid System** based on a 12-column architecture. Surfaces are aligned to a strict 4px baseline grid to maintain mathematical precision.

Margins and gutters are generous to prevent visual clutter, allowing the "circuit trace" decorative lines to flow between sections without overlapping critical data. The background layer should feature a subtle 20px x 20px "digital" dot grid to ground the UI elements in a simulated engineering canvas.

## Elevation & Depth

Depth is achieved through **Tonal Layering** and **Luminescent Borders** rather than traditional shadows. 
- **Level 0 (Background):** The deepest layer (#0A0A0A) featuring the dot grid.
- **Level 1 (Panels):** Semi-transparent surfaces (#121212 at 80% opacity) with a 1px solid border (#2A2A2A).
- **Level 2 (Active States):** Elements that are hovered or active gain a "Glowing Aura"—a 1px Neon Green border with a subtle 4px outer bloom (box-shadow: 0 0 8px rgba(57, 255, 20, 0.4)).

Glassmorphism is used sparingly for floating HUD overlays, utilizing a heavy backdrop-blur (12px) to maintain readability against busy circuit-pattern backgrounds.

## Shapes

The design system utilizes **Sharp (0px)** corners for all structural components, including cards, buttons, and input fields. This reinforces the industrial, machined nature of electronics hardware. 

The only exception to the 0px rule is for specific decorative "trace-line" junctions which may use 45-degree chamfered corners (clipped corners) to mimic the routing of high-speed signals on a Printed Circuit Board (PCB).

## Components

### Buttons
Primary buttons are solid black with a 1px Neon Green border. Upon hover, the "circuit activation" state triggers: the border glows, and the text gains a slight green outer-glow. Secondary buttons use a subtle gray border that turns Cyan on hover.

### Input Fields
Inputs are dark, recessed rectangles with "Space Grotesk" labels positioned above the field in all-caps. The focus state must highlight the entire perimeter in Neon Green.

### Chips & Status Indicators
Status chips use a "monolithic" look: small rectangles with high-contrast text. A "System Online" status should pulse slowly with a 2px green glow to indicate a heartbeat.

### Circuit Traces
A unique component for this design system: decorative 1px lines that connect various cards or sections. These lines should always be horizontal, vertical, or 45-degrees, mimicking PCB traces. They should occasionally feature a small "solder pad" (a 4px square) at intersection points.

### Cards
Cards are the primary data containers. They feature a "header-bar" that is 2px taller than the rest of the frame, often containing a technical serial number or ID in the top-right corner to enhance the "Midnight Laboratory" theme.