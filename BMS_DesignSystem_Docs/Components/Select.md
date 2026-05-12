# Select And Pickers

Figma sections:

- `4.4 选择器 / Select`
- `4.5 级联选择 / Cascader`
- `4.6 日期选择器 / DatePicker`
- `4.7 时间选择器 / TimePicker`
- `4.8 日期时间选择器 / DateTimePicker`

## Component Sets

| Component | Variants | Props |
|---|---:|---|
| `Select` | 11 | `Style`, `State` |
| `DropdownMenu` for Select | 2 | `Component`, `Type` |
| `Cascader` | 11 | `Style`, `State` |
| `DropdownMenu` for Cascader | 2 | `Component`, `Type` |
| `DatePicker` | 25 | `Style`, `State` |
| `DropdownMenu` for DatePicker | 5 | `Component`, `Type` |
| `TimePicker` | 10 | `Style`, `State` |
| `DropdownMenu` for TimePicker | 2 | `Component`, `Type` |
| `DateTimePicker` | 10 | `Component`, `State` |
| `DropdownMenu` for DateTimePicker | 3 | `Component`, `Type` |

## Shared States

`Default`, `Hover`, `Active`, `Unfocus`, `Disabled`

## Select Styles

`Single`, `Multiple`, `Multiple Fold`

## Picker Rules

- Use `Select` for known flat options.
- Use `Cascader` for hierarchical options.
- Use `DatePicker` for date and date range.
- Use `TimePicker` for time.
- Use `DateTimePicker` only when users must choose both date and time.
- Dropdown menu should be visually connected to the trigger.
- Disabled state should block interaction and use disabled text/border tokens.

## Filter Bar Rule

From Figma pattern:

- Single choice with 3 or fewer options: use `Radio`.
- Multiple choice with 4 or fewer options: use `Checkbox`.
- Multiple choice with more than 5 options: use `Select`.

