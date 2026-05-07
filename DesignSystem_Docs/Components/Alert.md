# Alert

## 使用场景

- 用于页面内重要提示。

## 允许变体

Info / Success / Warning / Error

## 尺寸与视觉

背景使用状态背景 Token；文字/图标使用状态 Token；尺寸、圆角：待定。

> 注意：未经 Token 确认的高度、内边距、圆角、行高、阴影均标记为“待定”，不得写成 Token。

## 状态

- default
- closable：待定

## 交互规则

- 提示内容必须简短明确。
- 错误类 Alert 必须给出下一步建议。

## 前端适配

```tsx
<Alert type="warning" message="请先完成配置" />
```

## 禁止事项

- 禁止将 Alert 当成普通内容容器。

## AI 生成约束

- 必须优先调用系统 `Alert` 组件。
- 禁止临时创建同类组件。
- 颜色必须来自 `Foundations/tokens.json` 或 `Foundations/tokens.css`。
- 未经 Token 确认的尺寸、圆角、行高不得写死为 Token；需要标记为“待定”或复用项目已有变量。
