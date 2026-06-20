---
name: Apex Velocity
colors:
  surface: '#121415'
  surface-dim: '#121415'
  surface-bright: '#38393a'
  surface-container-lowest: '#0c0e0f'
  surface-container-low: '#1a1c1d'
  surface-container: '#1e2021'
  surface-container-high: '#282a2b'
  surface-container-highest: '#333536'
  on-surface: '#e2e2e3'
  on-surface-variant: '#e6bdba'
  inverse-surface: '#e2e2e3'
  inverse-on-surface: '#2f3132'
  outline: '#ac8885'
  outline-variant: '#5c3f3d'
  surface-tint: '#ffb3ae'
  primary: '#ffb3ae'
  on-primary: '#68000b'
  primary-container: '#c0001e'
  on-primary-container: '#ffcdc9'
  inverse-primary: '#c0001e'
  secondary: '#ffb3af'
  on-secondary: '#68000d'
  secondary-container: '#ff5355'
  on-secondary-container: '#5c000a'
  tertiary: '#c8c6c8'
  on-tertiary: '#313032'
  tertiary-container: '#5f5e60'
  on-tertiary-container: '#dbd8da'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#ffdad7'
  primary-fixed-dim: '#ffb3ae'
  on-primary-fixed: '#410004'
  on-primary-fixed-variant: '#930014'
  secondary-fixed: '#ffdad7'
  secondary-fixed-dim: '#ffb3af'
  on-secondary-fixed: '#410005'
  on-secondary-fixed-variant: '#930017'
  tertiary-fixed: '#e5e1e4'
  tertiary-fixed-dim: '#c8c6c8'
  on-tertiary-fixed: '#1c1b1d'
  on-tertiary-fixed-variant: '#474649'
  background: '#121415'
  on-background: '#e2e2e3'
  surface-variant: '#333536'
typography:
  display-lg:
    fontFamily: Bebas Neue
    fontSize: 96px
    fontWeight: '400'
    lineHeight: 96px
    letterSpacing: 0.02em
  display-lg-mobile:
    fontFamily: Bebas Neue
    fontSize: 64px
    fontWeight: '400'
    lineHeight: 60px
  headline-xl:
    fontFamily: Bebas Neue
    fontSize: 60px
    fontWeight: '400'
    lineHeight: 60px
    letterSpacing: 0.03em
  headline-lg:
    fontFamily: Bebas Neue
    fontSize: 48px
    fontWeight: '400'
    lineHeight: 48px
  headline-md:
    fontFamily: Bebas Neue
    fontSize: 32px
    fontWeight: '400'
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
  data-label:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
    letterSpacing: 0.05em
  price-display:
    fontFamily: JetBrains Mono
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 24px
spacing:
  unit: 4px
  gutter: 24px
  margin-desktop: 80px
  margin-mobile: 20px
  section-gap: 120px
---

## Brand & Style

This design system is engineered for a high-performance motorcycle dealership, prioritizing authority, speed, and precision. The aesthetic is **Cinematic Minimalism** mixed with **High-Contrast Technical** elements. It targets enthusiasts who view motorcycles not just as transport, but as high-end machinery.

The visual narrative is "The Garage at Midnight"—deep blacks, sharp edges, and the aggressive glow of taillights. The UI should feel expensive, heavy, and mechanical. Use massive whitespace to frame product photography, treating every motorcycle like a piece of art. Transitions should be swift yet smooth, mimicking the acceleration of a liter-class engine.

## Colors

The palette is strictly nocturnal. The **Primary BG (#0A0A0C)** provides a deep, void-like canvas that allows product photography to pop. **Surface 1 (#111114)** is used for cards and structural containers to create subtle depth without breaking the dark aesthetic.

**Accent Red (#C0001E)** is used for primary actions and brand identifiers, while **Accent Red Glow (#FF0030)** is reserved for hover states, active indicators, and "live" statuses, mimicking the intensity of LED braking systems. Borders should utilize the red-tinted rgba value to create a "heat" effect around containers.

## Typography

Typography is a hierarchy of power and precision. **Bebas Neue** is used for all headlines; it should always be uppercase to maintain an authoritative, editorial look. On desktop, don't be afraid of massive "Display" sizes for hero sections.

**Inter** handles all narrative and descriptive text, providing a clean, neutral balance to the aggressive headlines. **JetBrains Mono** is the technical layer—use it for spec sheets, VIN numbers, pricing, and performance metrics (0-60 times, BHP, Torque) to evoke the feeling of a precision-tuned ECU readout.

## Layout & Spacing

This design system utilizes a **12-column fixed grid** on desktop (1440px max-width) and a **4-column fluid grid** on mobile. The spacing rhythm is based on a 4px scale, but leans heavily into large gaps (Section gaps of 120px+) to create a premium, uncrowded feel.

Content should feel "bolted" to the grid. Use asymmetrical layouts where images span 8 columns and text spans 4 to create dynamic, editorial compositions. On mobile, transition to a single-stack layout but maintain the aggressive 20px side margins to preserve the "frame" effect.

## Elevation & Depth

Depth is achieved through **Tonal Layering** rather than traditional drop shadows. 

1.  **Base:** #0A0A0C (Background).
2.  **Raised:** #111114 (Cards/Sections) with a 1px solid border of `rgba(192, 0, 30, 0.4)`.
3.  **Overlay:** Use deep, diffused shadows (0px 20px 40px rgba(0,0,0,0.8)) for modals and tooltips.

Motion is critical for perceived depth. Use the custom cubic-bezier `(0.16, 1, 0.3, 1)` for all hover states and page transitions. This "Out-Quart" curve creates a feeling of rapid movement that decelerates smoothly into place.

## Shapes

The shape language is **Industrial and Sharp**. A strict **2px corner radius** is applied across the entire system—from buttons to cards to input fields. This near-zero roundedness communicates structural integrity and mechanical precision. 

Avoid circles. If an icon or image requires a container, use a square or a diamond (45-degree rotated square) to maintain the aggressive silhouette.

## Components

### Buttons
- **Primary:** Solid #C0001E, white text (Inter Bold, All Caps), 2px radius. On hover, apply a box-shadow glow using #FF0030.
- **Secondary:** Ghost style. 1px border of #F4F4F5, no background. 
- **Action:** For "Book a Test Ride," use a slightly wider padding to emphasize importance.

### Cards
- Background: #111114.
- Border: 1px solid `rgba(192,0,30,0.4)`.
- Image: 1:1 or 16:9 aspect ratio, high-contrast, desaturated until hover.

### Input Fields
- Dark background (#050505), 1px bottom-border only of #A1A1AA. 
- Focus state: Bottom-border changes to #C0001E with a subtle red glow.

### Technical Data Tables
- Use **JetBrains Mono** for all content. 
- Alternating row highlights using #111114.
- Left-aligned labels, right-aligned values for maximum readability of specs.

### Navigation
- Top-bar: Transparent background that blurs/darkens on scroll. 
- Links: Inter Medium, All Caps, 12px, 0.1em letter spacing.