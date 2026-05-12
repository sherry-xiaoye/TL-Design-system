# Input

Figma section: `4.1 输入框 / Input`

## Component Set

| Component | Variants | Props |
|---|---:|---|
| `Input` | 15 | `Style`, `State` |

## Props

### Style

| Style | Usage |
|---|---|
| `Short` | Compact fields in filter bars or narrow forms |
| `Long` | Standard form fields |
| `Unit` | Numeric input with unit suffix |

### State

`Default`, `Hover`, `Active`, `Unfocus`, `Disabled`

## Usage

- Use `Input` for free text, number, ID, keyword, and search-like single-line entry.
- Use `Select` when users choose from known options.
- Use `DatePicker`, `TimePicker`, or `DateTimePicker` for time-based values.
- Use `Disabled` only when a field is unavailable and should not be edited.

## Layout

- Default height is 36px in page forms and filter bars.
- Pair label and control in a `label-item + control` structure.
- In form pages, fields often use widths of 360px or 480px.
- In filter bars, fields often use a 60px label plus 240px control.

## Validation

- Error text should be short and placed near the field.
- Required fields use a leading required mark in the label.
- Do not rely on placeholder text as the only label.

