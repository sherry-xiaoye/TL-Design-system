# General Guidelines

## Product Character

BMS is an operational system. The UI should feel:

- Dense but readable
- Stable and predictable
- Fast to scan
- Action-oriented
- Conservative with decoration

## Interaction

- Controls must have default, hover, active/focus, and disabled states where variants exist.
- Forms must expose validation and required states.
- Tables must support loading, empty, selected, and error states.
- Dialogs must support keyboard operation.

## Visual

- Use neutral surfaces and semantic status colors.
- Use brand blue for primary actions and active navigation.
- Use 4px spacing rhythm.
- Use 4px or 8px radius for most components.
- Keep icons aligned to text baselines.

## Content

- Use concise Chinese labels for BMS workflows.
- Button labels should be verbs: `查询`, `重置`, `新增`, `保存`, `取消`, `删除`, `导出`.
- Table column names should be nouns.
- Error messages should be actionable.

## Implementation

- Prefer composition over large monolithic components.
- Use controlled components for forms.
- Keep page templates separate from atomic components.
- Keep token mapping centralized.

