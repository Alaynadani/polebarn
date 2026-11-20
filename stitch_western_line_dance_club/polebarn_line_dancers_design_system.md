---
name: "Vintage Pioneer & Prairie"
description: "A heritage Americana frontier design system for the Polebarn Line Dancers, pairing deep prairie pine green, weathered aged parchment, warm antique gold, and distressed broadside borders."
---

## Overview

The Polebarn Line Dancers design system celebrates old-time western heritage—drawing inspiration from vintage frontier dance hall posters, weathered timber saloon notices, pine-studded prairie landscapes, and warm brass kerosene lamps.

The visual direction preserves the cherished old-time character and hospitality of the original dance hall while refreshing the color palette to deep frontier prairie pine, warm sunbaked wheat parchment, and rich burnished cider brass. The layout emphasizes an authentic broadside hierarchy with framed double-line borders, banner plaques, and clean editorial columns.

## Colors

The palette transitions to a grounded vintage prairie aesthetic:

- **Primary:** Deep Prairie Pine (`#1E3A2B`) providing rich, stately frontier contrast for headings, primary actions, and badges.
- **Secondary:** Aged Saddle Hickory (`#783E19`) for secondary actions, dance counts, and borders.
- **Accent:** Antique Kerosene Gold (`#D49B28`) for call-to-action highlights, stars, and spotlighted nights.
- **Surface:** Sunbleached Wheat Parchment (`#FAF7F0`) and Warm Prairie Board (`#F2ECE1`) offering an authentic weathered paper warmth.

```yaml
colors:
  accent: "#D49B28"
  secondary: "#783E19"
  border: "#DCD3C3"
  light:
    primary: "#1E3A2B"
    on-primary: "#FFFFFF"
    surface: "#FAF7F0"
    on-surface: "#1B221E"
    surface-container: "#F2ECE1"
    surface-container-high: "#E6DDCE"
    on-surface-variant: "#58625B"
  dark:
    primary: "#9CD7B7"
    on-primary: "#0B2618"
    surface: "#111A15"
    on-surface: "#E9F0EC"
    surface-container: "#1A2620"
    surface-container-high: "#24332B"
    on-surface-variant: "#AEC0B6"
```

## Typography

This system uses **Castoro** as an expressive, authentic western headline serif with traditional American broadside heritage, paired with **Merriweather Sans** for clear, open humanist body text and step-by-step dance instructions. **Spline Sans Mono** handles dance counts (32-count, 4-wall), BPMs, and event start times.

```yaml
typography:
  display-lg:
    fontFamily: "Castoro"
    fontSize: 48px
    fontWeight: 700
    lineHeight: 56px
    letterSpacing: -0.5px
  display-lg-mobile:
    fontFamily: "Castoro"
    fontSize: 32px
    fontWeight: 700
    lineHeight: 40px
    letterSpacing: -0.25px
  headline-lg:
    fontFamily: "Castoro"
    fontSize: 36px
    fontWeight: 700
    lineHeight: 44px
    letterSpacing: -0.25px
  headline-lg-mobile:
    fontFamily: "Castoro"
    fontSize: 28px
    fontWeight: 700
    lineHeight: 34px
  headline-md:
    fontFamily: "Castoro"
    fontSize: 24px
    fontWeight: 600
    lineHeight: 32px
  headline-sm:
    fontFamily: "Castoro"
    fontSize: 20px
    fontWeight: 600
    lineHeight: 28px
  title-lg:
    fontFamily: "Merriweather Sans"
    fontSize: 18px
    fontWeight: 700
    lineHeight: 26px
  body-lg:
    fontFamily: "Merriweather Sans"
    fontSize: 16px
    fontWeight: 400
    lineHeight: 24px
  body-md:
    fontFamily: "Merriweather Sans"
    fontSize: 14px
    fontWeight: 400
    lineHeight: 20px
  label-lg:
    fontFamily: "Merriweather Sans"
    fontSize: 14px
    fontWeight: 700
    lineHeight: 20px
  label-md:
    fontFamily: "Merriweather Sans"
    fontSize: 12px
    fontWeight: 600
    lineHeight: 16px
  mono-sm:
    fontFamily: "Spline Sans Mono"
    fontSize: 12px
    fontWeight: 500
    lineHeight: 16px
```

## Layout & Spacing

Layouts follow a fluid, responsive container system with a max width of 1280px on desktop and cozy touch-friendly gutters on mobile. Rhythms are spaced on an 8px scale.

```yaml
spacing:
  gutter-xs: 4px
  gutter-sm: 8px
  gutter-md: 16px
  gutter-lg: 24px
  gutter-xl: 32px
  section: 64px
  page-margin: 24px
```

## Elevation & Depth

Surfaces emphasize tactile natural layering rather than heavy artificial drop shadows. Borders feature warm subtle outlines (`#DCD3C3`) paired with soft ambient diffusion (`0 4px 20px -2px rgba(27, 34, 30, 0.08)`). Badges, cards, and banners feel like embossed leather patches and framed wooden placards.

## Shapes

Corners feature grounded, gently rounded corners (8px default, 16px on hero cards) reminiscent of sanded cedar planks, saddle stitch corners, and vintage event tickets.

```yaml
rounded:
  sm: 4px
  DEFAULT: 8px
  md: 12px
  lg: 16px
  xl: 24px
  full: 9999px
```

## Motion & Micro-interaction

Micro-interactions feel smooth, physical, and friendly—reminiscent of tactile tavern doors and responsive stepping. Transitions avoid snappy digital flashes.

```yaml
motion:
  state-change:
    duration: 150ms
    delay: 0ms
    timingFunction: ease-out
  surface-enter:
    duration: 250ms
    delay: 0ms
    timingFunction: cubic-bezier(0.2, 0, 0, 1)
  surface-exit:
    duration: 150ms
    delay: 0ms
    timingFunction: cubic-bezier(0.3, 0, 1, 1)
```

## Voice & Content Strategy

- **Tone:** Warm, communal, encouraging, and genuine. We speak with down-home hospitality without caricature. Absolute beginners are met with reassurance ("No partner needed, two left feet welcome!").
- **Terminology:** "Floor Call", "Step Sheet", "Wall Count", "BPM", "Social Stomp", "Open Floor", "Walkthrough", "Barn Night".
- **Action Labels:** Action-driven and descriptive: "View Step Sheet", "RSVP for Saturday Stomp", "Filter by Beginner Level", "Download Practice Track".

## Components

Component implementations live as individual HTML sticker sheet files in
`components/`. Each file contains the canonical, styled HTML components with
`<!-- COMPONENT: name -->` comment markers. Read each file before use.

- **Button** → `@components/button.html`: `button-primary`, `button-icon`, `button-with-icon`
- **Card** → `@components/card.html`: `card-elevated`, `card-action`, `card-interactive`, `card-interactive-2`
- **Table** → `@components/table.html`: `table-standard`, `table-interactive`, `table-selectable`
- **Tabs** → `@components/tabs.html`: `tabs-horizontal`, `tabs-with-icon`
