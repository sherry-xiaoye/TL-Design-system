# Card

## 使用场景

- 用于承载相对独立的信息区块。

## 允许变体

Default / WithHeader（待定）

## 尺寸与视觉

背景使用 `--bms-color-bg-white`；内边距、圆角、阴影：待定。

> 注意：未经 Token 确认的高度、内边距、圆角、行高、阴影均标记为“待定”，不得写成 Token。

## 状态

- default
- loading
- empty

## 交互规则

- 避免多层嵌套卡片。
- Card 内应有明确标题或内容结构。

## 前端适配

```tsx
<Card title="基础信息">...</Card>
```

## 禁止事项

- 禁止卡片层层嵌套。
- 禁止使用强阴影或大圆角。

## AI 生成约束

- 必须优先调用系统 `Card` 组件。
- 禁止临时创建同类组件。
- 颜色必须来自 `Foundations/tokens.json` 或 `Foundations/tokens.css`。
- 未经 Token 确认的尺寸、圆角、行高不得写死为 Token；需要标记为“待定”或复用项目已有变量。
