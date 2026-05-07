# Tag

## 使用场景

- 用于展示状态、分类、属性。

## 允许变体

Default / Success / Warning / Error / Info

## 尺寸与视觉

颜色使用状态 Token；尺寸、圆角：待定。

> 注意：未经 Token 确认的高度、内边距、圆角、行高、阴影均标记为“待定”，不得写成 Token。

## 状态

- default
- closable：待定

## 交互规则

- 状态类 Tag 必须使用语义色。
- 文案保持短。

## 前端适配

```tsx
<Tag type="success">已完成</Tag>
<Tag type="warning">待处理</Tag>
```

## 禁止事项

- 禁止随机生成 Tag 颜色。

## AI 生成约束

- 必须优先调用系统 `Tag` 组件。
- 禁止临时创建同类组件。
- 颜色必须来自 `Foundations/tokens.json` 或 `Foundations/tokens.css`。
- 未经 Token 确认的尺寸、圆角、行高不得写死为 Token；需要标记为“待定”或复用项目已有变量。
