# Popover

## 使用场景

- 用于承载轻量浮层内容。

## 允许变体

Hover / Click（待定）

## 尺寸与视觉

背景使用白色 Token；边框/阴影/圆角：待定。

> 注意：未经 Token 确认的高度、内边距、圆角、行高、阴影均标记为“待定”，不得写成 Token。

## 状态

- closed
- open

## 交互规则

- 内容不宜过复杂。
- 复杂表单不应放入 Popover。

## 前端适配

```tsx
<Popover content="说明内容"><Button>查看</Button></Popover>
```

## 禁止事项

- 禁止在 Popover 中放复杂编辑流程。

## AI 生成约束

- 必须优先调用系统 `Popover` 组件。
- 禁止临时创建同类组件。
- 颜色必须来自 `Foundations/tokens.json` 或 `Foundations/tokens.css`。
- 未经 Token 确认的尺寸、圆角、行高不得写死为 Token；需要标记为“待定”或复用项目已有变量。
