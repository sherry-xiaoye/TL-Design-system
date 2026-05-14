# Default

## 使用场景

- 用于记录通用组件默认规则。

## 允许变体

Default

## 尺寸与视觉

所有未确认尺寸标记为待定。颜色使用已确认 Token。

> 注意：未经 Token 确认的高度、内边距、圆角、行高、阴影均标记为“待定”，不得写成 Token。

## 状态

- default
- disabled
- loading
- empty
- error

## 交互规则

- 默认使用 Token 色值。
- 默认使用系统组件。

## 前端适配

```tsx
// 默认规则，不直接作为组件调用
```

## 禁止事项

- 禁止自定义非系统样式。

## AI 生成约束

- 必须优先调用系统 `Default` 组件。
- 禁止临时创建同类组件。
- 颜色必须来自 `Foundations/tokens.json` 或 `Foundations/tokens.css`。
- 未经 Token 确认的尺寸、圆角、行高不得写死为 Token；需要标记为“待定”或复用项目已有变量。
