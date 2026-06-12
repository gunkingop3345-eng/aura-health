---
name: Serene Cycle
colors:
  surface: '#fff8f7'
  surface-dim: '#e1d8d8'
  surface-bright: '#fff8f7'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#fbf1f1'
  surface-container: '#f5ecec'
  surface-container-high: '#f0e6e6'
  surface-container-highest: '#eae0e0'
  on-surface: '#1f1b1b'
  on-surface-variant: '#554241'
  inverse-surface: '#342f30'
  inverse-on-surface: '#f8eeee'
  outline: '#897271'
  outline-variant: '#dcc0bf'
  surface-tint: '#9e3f42'
  primary: '#9e3f42'
  on-primary: '#ffffff'
  primary-container: '#ff8a8a'
  on-primary-container: '#772126'
  inverse-primary: '#ffb3b1'
  secondary: '#894e4f'
  on-secondary: '#ffffff'
  secondary-container: '#ffb3b3'
  on-secondary-container: '#7b4243'
  tertiary: '#30628a'
  on-tertiary: '#ffffff'
  tertiary-container: '#81b1dc'
  on-tertiary-container: '#024469'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#ffdad8'
  primary-fixed-dim: '#ffb3b1'
  on-primary-fixed: '#410007'
  on-primary-fixed-variant: '#7f282c'
  secondary-fixed: '#ffdad9'
  secondary-fixed-dim: '#ffb3b3'
  on-secondary-fixed: '#370d10'
  on-secondary-fixed-variant: '#6d3738'
  tertiary-fixed: '#cde5ff'
  tertiary-fixed-dim: '#9bcbf8'
  on-tertiary-fixed: '#001d32'
  on-tertiary-fixed-variant: '#104a70'
  background: '#fff8f7'
  on-background: '#1f1b1b'
  surface-variant: '#eae0e0'
typography:
  display-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 40px
    fontWeight: '700'
    lineHeight: 48px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
  headline-lg-mobile:
    fontFamily: Plus Jakarta Sans
    fontSize: 28px
    fontWeight: '600'
    lineHeight: 36px
  headline-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  body-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
    letterSpacing: 0.01em
  label-sm:
    fontFamily: Plus Jakarta Sans
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 8px
  container-padding-mobile: 24px
  container-padding-desktop: 48px
  gutter: 16px
  section-gap: 32px
  stack-sm: 4px
  stack-md: 12px
  stack-lg: 24px
---

## Brand & Style
The design system is centered on empathy, clarity, and biological rhythm. It aims to transform a technical tracking task into a supportive, personal ritual. The aesthetic blends **Minimalism** with **Soft-Tactile** elements to create an environment that feels less like a medical log and more like a wellness companion.

Targeting users seeking a non-clinical, calming experience, the UI leverages generous whitespace to reduce cognitive load during sensitive times. The emotional response should be one of "gentle guidance"—providing essential health data without causing alarm or clutter.

## Colors
The palette is rooted in warmth and softness. The primary coral (`#FF8A8A`) is used for action states and the current cycle day, while the secondary soft pink (`#FFB3B3`) handles decorative elements and secondary buttons.

A specialized set of status tokens is defined for cycle tracking:
- **Flow Indicators:** A monochromatic scale of reds/corals to indicate intensity without looking clinical.
- **Fertility:** Soft blues and lavenders are used to contrast against the period-related pinks, making the "fertile window" distinct and easy to identify.
- **Backgrounds:** The primary background uses a warm neutral (`#FFF5F5`) rather than pure white to reduce eye strain and maintain a cozy, organic feel.

## Typography
This design system utilizes **Plus Jakarta Sans** for its approachable, modern, and slightly rounded character. The letterforms are friendly and highly legible, which is critical for glanceable data like dates and symptom logs.

Headlines use a tighter letter-spacing and semi-bold weights to provide a sense of structure. Body text is kept airy with a generous line-height to ensure a relaxed reading experience. For data-heavy views like calendars, the `label-sm` role provides high-contrast, uppercase metadata that remains legible at small scales.

## Layout & Spacing
The layout philosophy is based on a **Fluid Grid** with a 8px baseline rhythm. To emphasize the feeling of "personal space," the design system uses larger-than-average container margins (24px on mobile) to keep content away from the edges of the device.

Vertical stacks use three primary tiers:
- **Stack-sm (4px):** Linking labels to inputs or small icons to text.
- **Stack-md (12px):** Spacing between card content or list items.
- **Stack-lg (24px):** Separating logical groups or headings from content.

Horizontal spacing focuses on a flexible 4-column grid for mobile, allowing for easy selection of "symptom chips" or calendar dates.

## Elevation & Depth
Depth is conveyed through **Tonal Layers** and **Ambient Shadows**. Instead of traditional harsh shadows, this design system uses soft, wide-dispersion shadows tinted with the primary coral or a neutral mauve.

- **Level 0 (Base):** The neutral background.
- **Level 1 (Cards/Containers):** Elevated by a subtle white inner-glow and a soft 10% opacity drop shadow. This creates a "pillow-like" effect.
- **Level 2 (Active States/Floating Buttons):** Increased shadow blur and a slight scale increase (1.02x) to suggest the element is floating closer to the user.

Glassmorphism is used sparingly for navigation bars and modal overlays, employing a high-intensity backdrop blur (20px) to maintain focus while keeping the warm background colors visible.

## Shapes
The shape language is consistently **Rounded**, avoiding sharp corners to maintain the supportive and friendly aesthetic. 

- **Standard Elements:** Buttons, input fields, and cards use a 0.5rem (8px) radius.
- **Interactive Tokens:** Status indicators and chips use a pill-shaped (full-round) geometry to differentiate them from structural layout elements.
- **Calendar Cells:** These use a soft circular shape for the "current day" and a continuous "capsule" shape for multi-day windows like flow or fertility.

## Components
- **Buttons:** The primary button is a pill-shape with a subtle gradient (Primary to Secondary) and a soft drop shadow. Ghost buttons use a coral outline with a 10% opacity fill.
- **Symptom Chips:** Small, rounded-xl containers with an icon and label. When selected, the background shifts to the primary coral and the icon performs a subtle "bounce" animation.
- **Status Indicators (The "Cycle Bar"):** A horizontal progress bar that uses "Fertility Window" and "Flow" tokens. Transitions between phases are blurred/feathered rather than hard-cut to symbolize the gradual nature of hormonal shifts.
- **Cards:** Used for insights and daily summaries. They feature a white background with a very soft neutral border (`#FFEDED`) and high container padding (20px) to prevent data from feeling cramped.
- **Inputs:** Text fields use a soft-gray border that transforms into a coral glow when focused, reinforcing the tactile nature of the UI.