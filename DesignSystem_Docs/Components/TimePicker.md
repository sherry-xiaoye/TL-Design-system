# TimePicker

## 使用场景

- 用于选择时间。

## 允许变体

Time / TimeRange（待定）

## 尺寸与视觉

尺寸：待定。颜色使用系统 Token。

> 注意：未经 Token 确认的高度、内边距、圆角、行高、阴影均标记为“待定”，不得写成 Token。

## 状态

- default
- open
- selected
- disabled
- error

## 交互规则

- 必须明确时间格式。
- 与日期联合使用时优先考虑 DateTimePicker。

## 前端适配

```tsx
<TimePicker />
```

## 禁止事项

- 禁止用普通 Input 手写时间格式。

## AI 生成约束

- 必须优先调用系统 `TimePicker` 组件。
- 禁止临时创建同类组件。
- 颜色必须来自 `Foundations/tokens.json` 或 `Foundations/tokens.css`。
- 未经 Token 确认的尺寸、圆角、行高不得写死为 Token；需要标记为“待定”或复用项目已有变量。
