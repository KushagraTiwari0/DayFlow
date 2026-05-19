---
name: Paper & Ink Minimalism
colors:
  surface: '#fcf9f8'
  surface-dim: '#dcd9d9'
  surface-bright: '#fcf9f8'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f6f3f2'
  surface-container: '#f0eded'
  surface-container-high: '#eae7e7'
  surface-container-highest: '#e4e2e1'
  on-surface: '#1b1c1c'
  on-surface-variant: '#424844'
  inverse-surface: '#303030'
  inverse-on-surface: '#f3f0ef'
  outline: '#727973'
  outline-variant: '#c2c8c2'
  surface-tint: '#496455'
  primary: '#173124'
  on-primary: '#ffffff'
  primary-container: '#2d4739'
  on-primary-container: '#98b5a3'
  inverse-primary: '#b0cdbb'
  secondary: '#94492b'
  on-secondary: '#ffffff'
  secondary-container: '#fd9e79'
  on-secondary-container: '#773317'
  tertiary: '#2d2b23'
  on-tertiary: '#ffffff'
  tertiary-container: '#444138'
  on-tertiary-container: '#b2ada1'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#ccead6'
  primary-fixed-dim: '#b0cdbb'
  on-primary-fixed: '#062014'
  on-primary-fixed-variant: '#324c3e'
  secondary-fixed: '#ffdbce'
  secondary-fixed-dim: '#ffb59a'
  on-secondary-fixed: '#370d00'
  on-secondary-fixed-variant: '#763316'
  tertiary-fixed: '#e8e2d5'
  tertiary-fixed-dim: '#cbc6ba'
  on-tertiary-fixed: '#1e1c14'
  on-tertiary-fixed-variant: '#4a473d'
  background: '#fcf9f8'
  on-background: '#1b1c1c'
  surface-variant: '#e4e2e1'
typography:
  display:
    fontFamily: Playfair Display
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Playfair Display
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
  headline-lg-mobile:
    fontFamily: Playfair Display
    fontSize: 28px
    fontWeight: '700'
    lineHeight: 36px
  headline-md:
    fontFamily: Playfair Display
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  body-lg:
    fontFamily: DM Sans
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: DM Sans
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-sm:
    fontFamily: DM Sans
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  label-md:
    fontFamily: DM Sans
    fontSize: 12px
    fontWeight: '700'
    lineHeight: 16px
    letterSpacing: 0.05em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 8px
  container-padding: 24px
  gutter: 16px
  card-gap: 20px
---

## Brand & Style

The design system is rooted in the quiet focus of analog journaling, translated for a high-performance digital environment. It aims to evoke the tactile satisfaction of physical stationery—specifically the texture of high-grade parchment and the precision of a fine-tip ink pen. 

The aesthetic is **Tactile Minimalism**. It avoids the sterility of modern SaaS by introducing organic warmth through its color palette and subtle depth, while maintaining the functional efficiency of a professional tool. The target audience values intentionality and seeks a digital "haven" for productivity that feels grounded and permanent rather than ephemeral.

## Colors

The palette is inspired by natural materials and academic environments.

*   **Primary (Forest Green):** Used for primary actions, success states, and key navigational elements. It provides a sense of growth and calm.
*   **Secondary (Terracotta):** Reserved for highlights, active states, and call-to-outs. It acts as the "ink" that draws the eye to what is important.
*   **Parchment (Backgrounds):** Instead of pure white, we use a warm parchment (#F9F7F2). This reduces eye strain and reinforces the paper metaphor.
*   **Ink (Neutral):** A deep charcoal (#262626) is used for typography to ensure high legibility without the harshness of true black.

## Typography

This design system utilizes a high-contrast typographic pairing to balance elegance with utility.

**Playfair Display** is our editorial voice. Use it for page titles, section headers, and moments of reflection. It should feel like the printed header of a premium planner.

**DM Sans** is our functional workhorse. It is used for all body text, input fields, and UI metadata. It provides a clean, neutral counterpoint to the serif headings, ensuring the interface remains easy to scan even with high data density.

## Layout & Spacing

The layout philosophy follows a **Modular Grid** system. On the dashboard, components are treated as "Sticky Notes" or "Paper Scraps" arranged on a board.

*   **Grid Model:** A 12-column fluid grid for desktop, transitioning to a single-column stack for mobile.
*   **Sticky Note Layout:** On the main dashboard, cards do not need to be perfectly aligned to a rigid grid. A slight 0.5-degree to 1-degree random rotation can be applied to "Card" containers to enhance the tactile feel.
*   **Rhythm:** We use an 8px base unit. Margins are generous to allow the "parchment" to breathe, emphasizing a lack of clutter.

## Elevation & Depth

Visual hierarchy is achieved through **Ambient Shadows** and **Tonal Layers**.

*   **The Board:** The lowest layer is the Parchment background.
*   **The Notes (Cards):** Cards sit slightly above the board. Use a very soft, diffused shadow (`0px 4px 20px rgba(0,0,0,0.05)`) to suggest they are lying flat on the surface.
*   **Active Elements:** When a card is "lifted" or interacted with, the shadow should deepen and expand (`0px 12px 32px rgba(0,0,0,0.08)`), simulating a physical object being picked up.
*   **Lines:** Use subtle, dotted or dashed dividers (Primary Color at 20% opacity) to mimic the printed lines of a notebook, as seen in the reference imagery.

## Shapes

The shape language is primarily rectangular with **Soft Corners** (`roundedness: 1`). 

We avoid perfectly sharp 90-degree angles to prevent the UI from feeling cold, but we also avoid heavy rounding (pill shapes) to maintain the "cut paper" aesthetic. This subtle rounding mimics the slightly worn edges of a frequently used planner. Buttons and UI controls follow this same logic, feeling like small tabs or labels.

## Components

### Buttons
Primary buttons use the Forest Green background with Parchment text. They should feel like "pressed-in" stamps. Secondary buttons use an outline of the primary color or the Terracotta for specific CTAs.

### Sticky Cards
The cornerstone of the dashboard. Each card should have a solid header background (using Tertiary or lightened versions of Primary/Secondary) to categorize information. Mimic the spiral-bound look by adding a "perforated" top border or small circular icons that resemble punch-holes.

### Input Fields
Inputs should look like simple underlined spaces or boxed areas with dotted lines, reminiscent of the "To Do Lists" in the reference image. When focused, the bottom border thickens and changes to Forest Green.

### Lists & Checkboxes
Checkboxes are simple squares with a hand-drawn checkmark style when active. Lists use the DM Sans font with wide line-height to allow for "mental space."

### Daily Progress Tracker
A custom component mimicking the "Water Tracker" or "Habit Tracker" from the reference image. Use small, circular outlines that "fill" with a solid Terracotta ink blot when completed.