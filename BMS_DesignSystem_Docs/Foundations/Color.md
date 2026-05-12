# Color

Color tokens are split into primitive tokens and semantic tokens.

## Primitive Tokens

Use primitive tokens to define the palette. Product components should normally consume semantic tokens instead of primitive values directly.

### Blue

| Token | Value | Usage |
|---|---:|---|
| `Color/Blue/Blue-B1` | `#eef5ff` | Light brand surface |
| `Color/Blue/Blue-B2` | `#b0c7ff` | Light brand border/fill |
| `Color/Blue/Blue-B3` | `#6e98ff` | Hover brand |
| `Color/Blue/Blue-B4` | `#3d71ff` | Active brand |
| `Color/Blue/Blue-B5` | `#2460f5` | Primary brand |

### Neutral

| Token | Value | Usage |
|---|---:|---|
| `Color/White/White` | `#ffffff` | Surface, card background |
| `Color/White/White80%` | `#ffffffcc` | Overlay / translucent surface |
| `Color/Middle/Middle-N1` | `#f7f8f9` | Page background |
| `Color/Middle/Middle-N2` | `#f2f2f3` | Subtle background |
| `Color/Middle/Middle-N3` | `#ededef` | Divider / subtle border |
| `Color/Middle/Middle-N4` | `#e1e2e5` | Default border |
| `Color/Middle/Middle-N5` | `#c0c1c6` | Disabled icon/text |
| `Color/Middle/Middle-N6` | `#a0a1a2` | Placeholder / tertiary text |
| `Color/Middle/Middle-N7` | `#666666` | Secondary text |
| `Color/Middle/Middle-N8` | `#303133` | Primary text |

### Status

| Token | Value | Usage |
|---|---:|---|
| `Color/Green/Green-G1` | `#e8faf4` | Success background |
| `Color/Green/Green-G2` | `#97e0cf` | Success border |
| `Color/Green/Green-G3` | `#4fc5a8` | Success hover |
| `Color/Green/Green-G4` | `#0fbb82` | Success |
| `Color/Green/Green-G5` | `#1f967c` | Success active |
| `Color/Yellow/Yellow-Y1` | `#fff5e3` | Warning background |
| `Color/Yellow/Yellow-Y2` | `#facf90` | Warning border |
| `Color/Yellow/Yellow-Y3` | `#faaa48` | Warning hover |
| `Color/Yellow/Yellow-Y4` | `#f69825` | Warning |
| `Color/Yellow/Yellow-Y5` | `#ea8e1d` | Warning active |
| `Color/Red/Red-R1` | `#ffeeee` | Error background |
| `Color/Red/Red-R2` | `#ffb4b4` | Error border |
| `Color/Red/Red-R3` | `#fc8b8b` | Error hover |
| `Color/Red/Red-R4` | `#f96c6c` | Error |
| `Color/Red/Red-R5` | `#e95454` | Error active |

### Accent

| Token | Value | Usage |
|---|---:|---|
| `Color/Purple/Purple-P4` | `#907afd` | Chart/accent |
| `Color/Orange/Orange-O1` | `#ffefe2` | Orange subtle background |
| `Color/Orange/Orange-O4` | `#ff955f` | Orange accent |

## Semantic Tokens

Use semantic tokens in components and page implementation.

| Group | Tokens |
|---|---|
| Background | `Default`, `Disabled Filled`, `Brand`, `Sidebar`, `TableHeader`, `Top Navigation`, `Disabled Subtle`, `zebra`, `Info`, `Success`, `Warning`, `Error` |
| Text | `Primary`, `Secondary`, `Disabled`, `Thirdly`, `Inverse`, `brand`, `TableHeader`, `Warning`, `Success`, `Error` |
| Border | `Default`, `Hover`, `Active`, `Unfocus`, `Disabled`, `Table`, `Chart Axis` |
| Divider | `Default` |
| Icon | `Default`, `Secondary`, `Disabled`, `Brand`, `Info`, `Success`, `Warning`, `Error`, `Inverse`, `TableHeader` |
| Radius | semantic radius aliases |
| Charts | chart color aliases |
| Size | semantic size aliases |

## Rules

- Use `Text/Primary` for main labels and table primary content.
- Use `Text/Secondary` for descriptions, helper text, and secondary table content.
- Use `Text/Disabled` for disabled controls only.
- Use status colors consistently: Info = blue, Success = green, Warning = yellow/orange, Error = red.
- Page background should be subtle neutral, with white cards or table surfaces.
- Avoid one-off hex values in product code.

