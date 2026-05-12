# Naming Guidelines

## Component Naming

Use Figma component names as canonical names:

- `Button`
- `TextButton`
- `Button-Danger`
- `Button-Group`
- `Input`
- `Select`
- `DatePicker`
- `TimePicker`
- `DateTimePicker`
- `Table-Header`
- `Table-Cell`
- `Dialog-Body`
- `Menu-Item`
- `Step-Item`
- `Sidebar-Left`
- `BMS-Header`

## Variant Naming

Preserve Figma variant prop names:

- `Size`
- `Style`
- `State`
- `Type`
- `Component`
- `Show`
- `Color`
- `Alignment`
- `Count`
- `Last`

## Token Naming

Preserve slash-separated token names:

```text
Color/Blue/Blue-B5
Text/Primary
Background/Default
Spacing/4
Radius/2
```

## Code Naming Recommendation

When converting to code, keep a stable mapping:

```ts
const token = {
  color: {
    blue: { b5: '#2460f5' },
    text: { primary: 'var(--bms-text-primary)' }
  }
}
```

## Rules

- Do not rename variants casually.
- Fix obvious typos only in code-facing aliases, while documenting the Figma original. Example: `Unfcous` may map to `unfocused`.
- Keep internal component names consistent with Figma even if display labels are localized.

