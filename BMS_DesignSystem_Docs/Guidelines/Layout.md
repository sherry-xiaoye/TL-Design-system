# Layout Guidelines

## App Shell

```text
Header: 1440 x 56
Sidebar: 180 x 844
Body: 1260 x 844
Body padding: 20
Main content width: 1220
```

## Page Layout

- BMS pages should start with the actual working interface, not a landing page.
- Use dense but organized layouts.
- Prefer predictable toolbar/filter/table structure.
- Avoid oversized hero sections and marketing composition.
- Do not use decorative cards as page sections.

## Region Order

Common table page:

```text
Header
Sidebar
Body
  FilterBar
  TableHeaderActions
  Table
  Pagination
```

Common form page:

```text
Header
Sidebar
Body
  Title
  Step(optional)
  Container
  Footer actions
```

## Responsive Guidance

The source design is desktop-first. When adapting:

- Preserve header/sidebar/body hierarchy.
- Collapse sidebar only when the product explicitly requires mobile/tablet support.
- Keep table operations accessible.
- Do not scale typography with viewport width.
- Maintain 4px spacing rhythm.

