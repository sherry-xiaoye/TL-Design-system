# Navigation

Figma sections:

- `3.1 面包屑 / Breakcrum`
- `3.2 导航菜单 / Menu`
- `3.4 步骤条 / Steps`
- `Header`
- `Side`

## Component Sets

| Component | Variants | Props |
|---|---:|---|
| `Breadcrumb` | 4 | `Level` |
| `Breadcrumb-Item` | 2 | `State` |
| `Menu-Item` | 15 | `Style`, `State`, `Icon` |
| `Step-Item` | 12 | `State`, `Type`, `Last` |
| `BMS-Header` | 1 | shell header |
| `Sidebar-Left` | 1 | left navigation shell |

## Shell

- Header height: 56px.
- Sidebar width: 180px.
- Body starts at `x=180`, `y=56`.
- Sidebar menu items use icon + label when first-level navigation requires recognition.

## Menu-Item Props

| Prop | Values |
|---|---|
| `Style` | `First`, `Second`, `Third` |
| `State` | `Default`, `Hover`, `Active` |
| `Icon` | `True`, `False` |

## Step-Item Props

| Prop | Values |
|---|---|
| `State` | `Finish`, `Process`, `Wait` |
| `Type` | `Horizontal`, `Vertical` |
| `Last` | `True`, `False` |

## Rules

- Use breadcrumb for location hierarchy, not primary navigation.
- Use sidebar for persistent module navigation.
- Use steps for multi-step creation or approval flows.
- Active menu item must be visually distinct and use semantic brand/background tokens.
- Do not mix multiple active states in one navigation group.

