# AI Generation Rules

Use this file as the main instruction file for Cursor when generating BMS UI from the Figma design system.

## Hard Rules

1. Use existing design-system components and variants before creating new UI.
2. Use tokens from `Foundations` before hard-coded CSS values.
3. Preserve BMS desktop shell: `BMS-Header`, `Sidebar-Left`, `Body`.
4. Build the real operational screen, not a marketing page.
5. Use dense, scannable, work-focused layouts.
6. Do not add decorative gradients, floating cards, oversized hero sections, or unrelated imagery.
7. Do not nest cards inside cards.
8. Do not show Toolbar and BulkActionBar at the same time.
9. Use one primary button per action area.
10. Use `Button-Danger` for destructive actions.

## Component Selection

| Need | Use |
|---|---|
| Main action | `Button` with `Style=Primary` |
| Secondary action | `Button` with `Style=Secondary` or `General` |
| Destructive action | `Button-Danger` |
| Inline action | `TextButton` or `Link` |
| Text input | `Input` |
| Flat option list | `Select` |
| Hierarchical options | `Cascader` |
| Date | `DatePicker` |
| Time | `TimePicker` |
| Date and time | `DateTimePicker` |
| Boolean setting | `Switch` |
| Multi-select | `Checkbox` |
| Single visible option group | `Radio` |
| Table actions | `TableHeaderActions` |
| Row selection actions | `BulkActionBar` pattern |
| Modal | `Dialog-Body` |
| Feedback | `Alert`, `Notification`, `Toast`, `Result` |

## Page Generation Checklist

For table pages:

- Header
- Sidebar
- FilterBar
- TableHeaderActions
- Table
- Pagination
- Empty/loading/error states

For form pages:

- Header
- Sidebar
- Title
- Optional steps
- Form container
- Footer actions
- Validation states

For dashboard pages:

- Header
- Sidebar
- Metric cards
- Chart grid
- Optional table/list details
- Loading/empty states

## Code Output Expectations

- Components should expose props matching Figma variant names.
- Use semantic prop names in code, but keep mapping to Figma variants.
- Keep CSS tokenized.
- Avoid one-off pixel values except documented shell sizes.
- Include keyboard and disabled states for interactive controls.

