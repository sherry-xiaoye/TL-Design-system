# Detail Page

Detail pages are not represented as a single named component set, but should be composed from the same shell, title, card, table, dialog, and form patterns.

## Recommended Structure

```text
Body
  Title / status tag / primary actions
  Summary card
  Detail sections
  Related table
  Operation log or timeline
```

## Components

- `BMS-Header`
- `Sidebar-Left`
- `Title`
- `Tag`
- `Card`
- `Table-Header`
- `Table-Cell`
- `Timeline`
- `Button`
- `Dialog-Body`

## Rules

- Put entity identity and status in the first viewport.
- Use sections for grouped information.
- Use tables for related records and operation logs.
- Use dialogs only for focused confirmation or short edit actions.
- For destructive actions, use `Button-Danger`.

