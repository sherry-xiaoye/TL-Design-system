# Typography

The Figma file defines 7 local text styles grouped into Chart, Heading, and Body.

## Text Styles

| Style | Size | Intended Usage |
|---|---:|---|
| `Chart/大字号` | 28 | Large numeric dashboard metric |
| `Chart/主要文本` | 20 | Primary chart metric text |
| `Heading/主页面和弹窗的标题` | 16 | Page title, dialog title |
| `Heading/页面内容的标题` | 14 | Section title, card title, table block title |
| `Heading/弹窗内容标题` | 12 | Dialog subsection heading |
| `Body/次文本` | 14 | Secondary body text |
| `Body/文本` | 12 | Default dense BMS UI text |

## Typography Rules

- BMS screens are dense operational interfaces. Prefer 12px and 14px body text.
- Use 16px only for page-level titles and modal titles.
- Use 28px only for dashboard metrics or chart numbers.
- Keep labels concise. Avoid long explanatory text inside controls.
- Use consistent line height from the text style; do not invent per-component line heights.
- Do not scale font size with viewport width.
- Letter spacing should be `0` unless a local text style explicitly requires otherwise.

## Recommended Mapping

| UI Surface | Text Style |
|---|---|
| Page title | `Heading/主页面和弹窗的标题` |
| Dialog title | `Heading/主页面和弹窗的标题` |
| Card title | `Heading/页面内容的标题` |
| Form label | `Body/文本` |
| Table cell | `Body/文本` |
| Secondary helper text | `Body/次文本` |
| Dashboard metric | `Chart/大字号` |

