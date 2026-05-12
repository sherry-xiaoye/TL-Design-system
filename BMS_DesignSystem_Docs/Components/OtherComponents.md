# Other Components

This file covers component sets that do not have dedicated Markdown files.

## Data Entry

| Component | Variants | Props |
|---|---:|---|
| `Radio` | 4 | `State` |
| `Checkbox` | 5 | `Property 1` |
| `Stepper` | 5 | `State` |
| `Switch` | 8 | `Style`, `State`, `Show` |
| `Upload` | 3 | `Style` |

### Radio

States: `Default`, `Disabled`, `Selected`, `SelectedDisabled`.

Use for mutually exclusive options. Prefer radio when option count is small and options should be visible.

### Checkbox

States observed: `Normol`, `Select`, `Disable`, `SelectDisable`, `Selectpart`.

Use for multi-select choices and table row selection.

### Stepper

States: `Default`, `Hover`, `Active`, `Unfcous`, `Disabled`.

Use for bounded numeric increments.

### Switch

Props:

- `Style`: `Large`, `Small`
- `State`: `Default`, `Disabled`
- `Show`: `On`, `Off`

Use for immediate binary settings.

### Upload

Styles: `Button`, `Page`, `Picture`.

Use `Button` for compact upload, `Page` for document upload, and `Picture` for image upload.

## Content

| Component | Variants | Props |
|---|---:|---|
| `Card` | 2 | `State` |
| `Title` | 3 | `State` |
| `Tag` | 5 | `Color` |
| `Timeline` | 1 | pattern |
| `Popover` | 1 | pattern |
| `Tooltip` | 1 | pattern |
| `Pagination` | 2 | `Style` |

### Card

States: `Default`, `Hover`.

Use cards for repeated content items and dashboard blocks. Do not nest cards inside cards.

### Title

States: `Large`, `Middle`, `Little`.

Use to structure content sections.

### Tag

Colors: `Gray`, `Blue`, `Green`, `Orange`, `Red`.

Use tags for status or category labels.

### Pagination

Styles: `Number`, `Select`.

Use `Number` for standard table pagination and `Select` when page size selection is needed.

