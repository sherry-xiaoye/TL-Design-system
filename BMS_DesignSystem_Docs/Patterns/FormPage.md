# Form Page

Figma examples:

- `表单/新建表单-step1`
- `表单/新建表单-step2`
- `表单/新建表单-step3`
- `表单/编辑表单`
- `复杂表单`

## Shell

```text
BMS-Header: 56px
Sidebar-Left: 180px
Body: x=180, y=56, width=1260, height=844
```

## Standard Form Page Structure

```text
Body
  Title
  Optional Step
  Container
    Form fields
    Upload / Select / Input / Date controls
  Footer Button-Group
```

## Field Layout

- Simple forms can use centered 480px fields.
- Complex forms can use multiple 360px columns.
- Label row uses required marker plus title.
- Input row follows label with 8px vertical gap.

## Multi-Step Form

Use `Step-Item` in horizontal mode.

Step states:

- Completed step: `Finish`
- Current step: `Process`
- Future step: `Wait`

## Footer

- Use fixed footer button group for edit/create flows.
- Primary action on the right.
- Secondary action on the left.

## Rules

- Use page forms for complex editing; avoid placing complex forms in dialogs.
- Required fields must show required mark.
- Do not use placeholder as label.
- Keep form labels concise.
- Use `Upload` for file/picture sections.

