# Table Page

Figma examples:

- `列表页/表格/基础表格`
- `列表页/表格/标准表格`
- `列表页/表格/高级表格`
- `列表页/表格/高级表格-列设置`

## Standard Structure

```text
Body
  Filter-Bar
  TableHeaderActions
  Table
  Pagination
  Optional ColumnSettings drawer
```

## Filter-Bar

Rules from Figma:

- Single choice with 3 or fewer options: `Radio`
- Multiple choice with 4 or fewer options: `Checkbox`
- Multiple choice with more than 5 options: `Select`
- Must contain `Reset` and `Search`
- Layout: left filters, right actions

Variants:

- `Fields=Simple, Advanced=False`
- `Fields=Medium, Advanced=False`
- `Fields=Complex, Advanced=True`
- `Fields=Complex, Advanced=False`

## TableHeaderActions

Default toolbar:

- Left: primary action and secondary actions
- Right: column settings, sort, text tools, filter toggle

Selected state:

- Replace toolbar with bulk action bar
- Show selected count
- Provide batch operations

## Column Settings

Use side panel layout:

- Header title + close icon
- Column list
- Width input
- Freeze checkbox
- Display switch
- Footer button group

## Rules

- Do not show Toolbar and BulkActionBar together.
- Keep table operation density high.
- Use `Table-Header` and `Table-Cell` variants.
- Provide empty, loading, and error states for generated table pages.

