# Table

Figma sections:

- `5.6 表格 / Table`
- `TableHeaderActions`

## Component Sets

| Component | Variants | Props |
|---|---:|---|
| `Table-Header` | 5 | `Style` |
| `Table-Cell` | 6 | `State` |
| `TableHeaderActions` | 4 | `Left Actions`, `Right Tools`, `State` |
| `ColumnSettings` | 1 | panel pattern |
| `Sort` | 1 | panel pattern |

## Table Header Styles

`Default`, `Money`, `Checkbox`, `Empty`, `Action`

## Table Cell States

`Simple`, `Complex`, `Icon`, `Money`, `Checkbox`, `Action`

## Toolbar Rules

Toolbar is the table operation area.

Structure:

```text
[Left Actions]                            [Right Utility]
Primary action / secondary actions         Column settings / Sort / Filter toggle
```

Rules:

- Left action area carries business actions.
- Only one primary action is allowed.
- Other left actions should be neutral or subtle.
- Right utility area is for data controls, not main business actions.
- Right utility aligns to the right.
- Use `Spacing/4` between right utility items.

## Selection State

When rows are selected:

- Replace the default toolbar with `BulkActionBar`.
- Show selected count.
- Provide batch actions such as delete or export.
- Provide select all and clear selection controls.
- Do not show Toolbar and BulkActionBar at the same time.

## ColumnSettings

Purpose: configure column visibility, order, frozen state, and width.

Structure:

- Field label
- Column width input
- Sort/order input
- Freeze checkbox
- Display switch
- Reset button
- Save button

## Sort

Purpose: configure table sort priority.

Structure:

- Field list
- Ascending control
- Descending control
- Clear sort
- Reset button
- Save button

## AI Generation Contract

- Always render empty, loading, selected, and normal table states.
- Keep row actions compact.
- Use `Table-Header` and `Table-Cell` variants instead of custom table styling.
- For advanced tables, include `Filter-Bar`, `TableHeaderActions`, table body, pagination, and optional column settings drawer.

