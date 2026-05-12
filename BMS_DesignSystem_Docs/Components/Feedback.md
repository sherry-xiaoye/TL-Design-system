# Feedback Components

Figma sections:

- `7.1 警告提示 / Alert`
- `7.2 通知提醒框 / Notification`
- `7.4 进度条 / Progress`
- `7.5 等待 / Loading`
- `7.6 轻提示 / Toast`
- `7.7 缺省图 / default`
- `结果反馈`

## Component Sets

| Component | Variants | Props |
|---|---:|---|
| `Alert` | 6 | `Style`, `State` |
| `Notification` | 4 | `Type` |
| `Progress` | 5 | `Type`, `Action` |
| `Loading` | 2 | `Style` |
| `Toast` | 6 | `State`, `Closable` |
| `Default-Image` | 4 | `State` |
| `Result` | 2 | `State` |

## Status Types

Use consistent status mapping:

| Status | Usage |
|---|---|
| `Info` | Neutral informational message |
| `Success` | Completed action or positive result |
| `Warning` | Risk, incomplete data, or reversible concern |
| `Error` | Failed action or blocking error |

## Alert

- Use in-page for persistent contextual messages.
- Variants include icon, link, and button patterns.
- Keep message short and actionable.

## Notification

- Use for async system feedback.
- Should not block page operation.

## Toast

- Use for transient action feedback.
- Closable variants exist; use close only for longer toast visibility.

## Default-Image

States: `Empty`, `404`, `AccessDenied`, `Error`.

## Result

States: `Success`, `Error`.

Use on submission completion, result pages, or high-emphasis feedback states.

