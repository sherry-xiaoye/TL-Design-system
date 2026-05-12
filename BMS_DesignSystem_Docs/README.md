# BMS DesignSystem Docs

This documentation package is generated from the read-only Figma file `TL DesignSystem(v3.0)` for Cursor and AI-assisted component generation.

Figma source:

`https://www.figma.com/design/hKW1ir899ubJy29DHseYI1/TL-DesignSystem%EF%BC%88v3.0%EF%BC%89`

## Structure

```text
BMS_DesignSystem_Docs/
  README.md
  Foundations/
    Color.md
    Typography.md
    Spacing.md
    Grid.md
    Icons.md
  Components/
    Button.md
    Input.md
    Table.md
    Dialog.md
    Select.md
    Navigation.md
    Feedback.md
    OtherComponents.md
  Patterns/
    FormPage.md
    TablePage.md
    DashboardPage.md
    DetailPage.md
  Guidelines/
    Layout.md
    Naming.md
    Grid.md
    AI_Generation_Rules.md
    Guidelines.md
```

## Figma Pages

| Page | Purpose |
|---|---|
| `Foundations / 基础` | Primitive tokens, semantic tokens, typography styles, icons |
| `Components / 组件` | Component sets and variants |
| `Patterns / 结构规则` | Layout patterns, page templates, filter bars, table actions, dashboard examples |

## Core Principles

- Use tokens before hard-coded values.
- Prefer semantic tokens in product UI, and primitive tokens only when defining the theme layer.
- Build dense, operational BMS interfaces rather than marketing layouts.
- Use existing component variants instead of inventing new states.
- Keep page layout based on header, left sidebar, body, filter bar, toolbar, table/card/detail content, and footer actions.
- Do not create decorative UI that is not represented in the design system.

## Cursor Usage

When asking Cursor to generate code, include the relevant files from this package:

- Global theme: `Foundations/Color.md`, `Foundations/Typography.md`, `Foundations/Spacing.md`
- Component implementation: one or more files from `Components/`
- Page generation: one file from `Patterns/` plus `Guidelines/AI_Generation_Rules.md`
- Naming and structure: `Guidelines/Naming.md`, `Guidelines/Layout.md`

