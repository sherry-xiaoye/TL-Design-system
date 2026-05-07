# Progress

## 使用场景

- 用于上传、导入、批处理进度展示。

## 允许变体

Line / Circle（待定）

## 尺寸与视觉

进度色优先使用品牌色或状态色 Token；尺寸：待定。

> 注意：未经 Token 确认的高度、内边距、圆角、行高、阴影均标记为“待定”，不得写成 Token。

## 状态

- processing
- success
- error

## 交互规则

- 必须展示当前状态。
- 失败状态必须提供错误原因或重试入口。

## 前端适配

```tsx
<Progress percent={percent} status="processing" />
```

## 禁止事项

- 禁止只展示动画但无进度或状态说明。

## AI 生成约束

- 必须优先调用系统 `Progress` 组件。
- 禁止临时创建同类组件。
- 颜色必须来自 `Foundations/tokens.json` 或 `Foundations/tokens.css`。
- 未经 Token 确认的尺寸、圆角、行高不得写死为 Token；需要标记为“待定”或复用项目已有变量。
