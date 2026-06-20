---
name: Sonic Noir
colors:
  surface: '#0b1326'
  surface-dim: '#0b1326'
  surface-bright: '#31394d'
  surface-container-lowest: '#060e20'
  surface-container-low: '#131b2e'
  surface-container: '#171f33'
  surface-container-high: '#222a3d'
  surface-container-highest: '#2d3449'
  on-surface: '#dae2fd'
  on-surface-variant: '#cbc3d7'
  inverse-surface: '#dae2fd'
  inverse-on-surface: '#283044'
  outline: '#958ea0'
  outline-variant: '#494454'
  surface-tint: '#d0bcff'
  primary: '#d0bcff'
  on-primary: '#3c0091'
  primary-container: '#a078ff'
  on-primary-container: '#340080'
  inverse-primary: '#6d3bd7'
  secondary: '#4cd7f6'
  on-secondary: '#003640'
  secondary-container: '#03b5d3'
  on-secondary-container: '#00424e'
  tertiary: '#ffb869'
  on-tertiary: '#482900'
  tertiary-container: '#ca801e'
  on-tertiary-container: '#3f2300'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#e9ddff'
  primary-fixed-dim: '#d0bcff'
  on-primary-fixed: '#23005c'
  on-primary-fixed-variant: '#5516be'
  secondary-fixed: '#acedff'
  secondary-fixed-dim: '#4cd7f6'
  on-secondary-fixed: '#001f26'
  on-secondary-fixed-variant: '#004e5c'
  tertiary-fixed: '#ffdcbb'
  tertiary-fixed-dim: '#ffb869'
  on-tertiary-fixed: '#2c1700'
  on-tertiary-fixed-variant: '#673d00'
  background: '#0b1326'
  on-background: '#dae2fd'
  surface-variant: '#2d3449'
typography:
  headline-xl:
    fontFamily: Montserrat
    fontSize: 40px
    fontWeight: '800'
    lineHeight: 48px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Montserrat
    fontSize: 28px
    fontWeight: '700'
    lineHeight: 34px
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: Montserrat
    fontSize: 24px
    fontWeight: '700'
    lineHeight: 30px
  headline-md:
    fontFamily: Montserrat
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
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
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '600'
    lineHeight: 20px
    letterSpacing: 0.05em
  label-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
    letterSpacing: 0.02em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  container-margin: 20px
  gutter: 16px
  stack-sm: 8px
  stack-md: 16px
  stack-lg: 32px
  section-gap: 48px
---

## Brand & Style

The design system is engineered for a premium, high-energy music streaming experience. It centers on a **Modern High-Contrast Dark** aesthetic, blending the depth of night with the electric pulse of live performance. The brand personality is immersive, sophisticated, and kinetic, designed to disappear behind the album art while providing a high-octane navigation experience.

The visual style utilizes a mix of **Glassmorphism** for persistent UI elements (like the player bar) and **Minimalism** for content-heavy views. This ensures that while the interface feels cutting-edge and layered, it never distracts from the core auditory experience. High-contrast accents are used sparingly but vibrantly to guide the user's eye to primary actions and active states.

## Colors

The palette is anchored by a "True Dark" foundation to preserve battery life on OLED screens and provide maximum contrast for the accent colors.

- **Primary (Electric Violet):** Used for primary buttons, active playback progress, and branding moments.
- **Secondary (Neon Cyan):** Used for secondary highlights, "New" badges, and specific genre-based accents.
- **Neutral/Background:** A spectrum of deep charcoals and navy-blacks (`#020617`) to create depth without using pure black, which can cause smearing during scrolling.
- **High Contrast:** Pure white and light silver are reserved for primary headers and active labels to ensure legibility against the dark canvases.

## Typography

This design system uses a dual-font strategy to balance character with utility. 

**Montserrat** is used for headlines to provide a bold, geometric, and energetic feel that resonates with music culture. It should be set with tighter letter-spacing for large titles to maintain a modern look.

**Inter** is the workhorse for all functional text. Its neutral, systematic nature ensures that track titles, artist names, and settings remain highly legible at small sizes. 

- Use **Headline XL** for artist profiles and featured playlists.
- Use **Label MD** in all-caps for small eyebrows or category headers to create a distinct visual hierarchy against body text.

## Layout & Spacing

The layout follows a **Fluid Grid** model optimized for mobile-first interaction. 

- **Margins:** A standard 20px horizontal margin is applied to all screens to ensure content doesn't bleed into the edges of modern curved displays.
- **Rhythm:** An 8px linear scale is used for all spacing. 
- **Horizontal Scrolling:** For the Home dashboard, use overflowing carousels for albums and playlists, allowing the "next" item to be partially visible (peeking) to encourage discovery.
- **Touch Targets:** All interactive elements (play buttons, menu dots) must maintain a minimum 44x44px hit area regardless of their visual size.

## Elevation & Depth

Hierarchy is established through a combination of **Tonal Layering** and **Glassmorphism**:

- **Level 0 (Base):** The darkest color (`#020617`), used for the main background.
- **Level 1 (Cards):** Slightly lighter surface (`#1E293B`) with a very soft, 10% opacity shadow to create a subtle lift.
- **Level 2 (Overlays):** Glassmorphic surfaces using a `backdrop-filter: blur(20px)` and a semi-transparent white border (1px, 10% opacity) to simulate the edge of glass. This is the primary style for the bottom player bar and navigation overlays.
- **Gradients:** Use subtle radial gradients (Primary color to transparent) in the background of Detail views to create a "spotlight" effect behind album art.

## Shapes

The shape language is consistently "Soft-Rounded." 

- **Standard Cards:** Use a 16px radius (`rounded-lg`) to create a friendly but modern feel.
- **Buttons:** Primary buttons should use the **Pill-shaped** (full radius) style to differentiate them from content cards.
- **Album Art:** Should maintain the 16px radius to match the UI, rather than being sharp-edged, to keep the aesthetic cohesive.
- **Inputs:** Search bars and text fields use a 12px radius for a slightly more structured look compared to buttons.

## Components

- **Buttons:** 
  - *Primary:* Electric Violet background, white text, pill-shaped.
  - *Secondary:* Ghost style with 1px Neon Cyan border or subtle glass background.
- **Player Bar:** A persistent glassmorphic strip at the bottom. It features minimalist stroke-based icons for Play/Pause and Skip. The progress bar is a thin 2px line, with the primary violet color indicating progress.
- **Music Cards:** Vertical stack with the image (16px radius) on top, followed by the track title in **Body MD** (White) and artist in **Label SM** (Secondary Text).
- **Upload Screen:** Features a large "Drop Zone" with a dashed 2px stroke in Secondary color and a glassmorphic background to suggest interactivity.
- **Icons:** Use a consistent 2px stroke weight. Icons should be "hollow" in their default state and "filled" when active or selected.
- **Chips:** Small, pill-shaped elements with a deep surface color and light text, used for genre filtering or mood tags.