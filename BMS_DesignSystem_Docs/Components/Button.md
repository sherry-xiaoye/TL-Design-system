# Button

Figma section: `2.1按钮/Button`

## Component Sets

| Component | Variants | Props |
|---|---:|---|
| `Button` | 36 | `Size`, `Style`, `State` |
| `TextButton` | 8 | `Style`, `State` |
| `Link` | 8 | `Style`, `State` |
| `Button-Danger` | 8 | `Size`, `State` |
| `Button-Group` | 4 | `Alignment`, `Count` |

## Button Props

### Size

| Size | Height | Usage |
|---|---:|---|
| `Large` | 36 | Primary page actions, footer actions |
| `Middle` | 30 | Default dense toolbar usage |
| `Small` | 24 | Compact table row actions |

### Style

| Style | Usage |
|---|---|
| `Primary` | One main action per area |
| `Secondary` | Secondary action with visual emphasis |
| `General` | Neutral action |

### State

`Default`, `Hover`, `Active`, `Disabled`

## Button-Danger

Use `Button-Danger` for destructive actions such as delete, remove, revoke, or cancel irreversible operation.

## Rules

- Only one primary button is allowed in a toolbar or dialog footer.
- Put destructive actions away from primary confirm actions when possible.
- Use `TextButton` or `Link` for low-emphasis inline actions.
- Use `Button-Group` for aligned footer actions or paired actions.
- Do not use primary style for navigation-only actions.

## AI Generation Contract

```ts
type ButtonSize = 'Large' | 'Middle' | 'Small';
type ButtonStyle = 'Primary' | 'Secondary' | 'General';
type ButtonState = 'Default' | 'Hover' | 'Active' | 'Disabled';
```

