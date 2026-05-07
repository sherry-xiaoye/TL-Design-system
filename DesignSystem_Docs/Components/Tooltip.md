# Tooltip

## 使用场景

- 用于短文本解释、超长文本完整展示。

## 允许变体

Default

## 尺寸与视觉

尺寸、背景、圆角：待定。

> 注意：未经 Token 确认的高度、内边距、圆角、行高、阴影均标记为“待定”，不得写成 Token。

## 状态

- hidden
- visible

## 交互规则

- 表格超长文本应 ellipsis + Tooltip。
- Tooltip 内容应简短。

## 前端适配

```tsx
<Tooltip title={fullText}><span>{shortText}</span></Tooltip>
```

## 禁止事项

- 禁止用 Tooltip 放复杂内容或操作。

## AI 生成约束

- 必须优先调用系统 `Tooltip` 组件。
- 禁止临时创建同类组件。
- 颜色必须来自 `Foundations/tokens.json` 或 `Foundations/tokens.css`。
- 未经 Token 确认的尺寸、圆角、行高不得写死为 Token；需要标记为“待定”或复用项目已有变量。
