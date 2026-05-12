# Dialog

Figma section: `7.3 对话框 / Dialog box`

## Component Set

| Component | Variants | Props |
|---|---:|---|
| `Dialog-Body` | 2 | `Style` |

## Style

| Style | Usage |
|---|---|
| `Primary` | Standard dialog with full title/content/footer structure |
| `Lightweight` | Lightweight confirmation or compact message dialog |

## Structure

```text
Dialog
  Header: title + close icon
  Body: content, forms, warnings, or result summary
  Footer: secondary action + primary action
```

## Rules

- Dialog title uses `Heading/主页面和弹窗的标题`.
- Footer should contain one primary action and one secondary action when confirmation is required.
- Put destructive confirmation in `Button-Danger`.
- Avoid long forms inside dialogs; use page forms for complex editing.
- Close icon uses the Figma `Icon` component with `Name=close` or equivalent.

## Accessibility

- Trap focus inside dialog.
- Escape closes only when data loss is not possible.
- Confirm button should be reachable by keyboard.
- Use clear action labels: `保存`, `确认`, `取消`, `删除`.

