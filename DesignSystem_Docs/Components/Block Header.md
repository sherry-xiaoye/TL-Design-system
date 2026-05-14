# Block Header

## 使用场景

- 用于区块标题和区块级操作。

## 允许变体

Title / TitleWithAction（待定）

## 尺寸与视觉

标题字号、间距：待定。文本颜色使用主文本 Token。

> 注意：未经 Token 确认的高度、内边距、圆角、行高、阴影均标记为“待定”，不得写成 Token。

## 状态

- default

## 交互规则

- 标题文案简短。
- 右侧可放置次要操作。

## 前端适配

```tsx
<BlockHeader title="基础信息" actions={<Button>编辑</Button>} />
```

## 禁止事项

- 禁止使用过大标题。
- 禁止装饰性标题样式。

## AI 生成约束

- 必须优先调用系统 `Block Header` 组件。
- 禁止临时创建同类组件。
- 颜色必须来自 `Foundations/tokens.json` 或 `Foundations/tokens.css`。
- 未经 Token 确认的尺寸、圆角、行高不得写死为 Token；需要标记为“待定”或复用项目已有变量。
