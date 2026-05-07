# Notification

## 使用场景

- 用于全局通知。

## 允许变体

Info / Success / Warning / Error

## 尺寸与视觉

背景、边框、阴影、位置、尺寸：待定；状态颜色使用 Token。

> 注意：未经 Token 确认的高度、内边距、圆角、行高、阴影均标记为“待定”，不得写成 Token。

## 状态

- open
- closed

## 交互规则

- 异步操作完成后可使用。
- 错误通知必须可理解。

## 前端适配

```tsx
notification.success({ message: "保存成功" })
```

## 禁止事项

- 禁止连续弹出大量 Notification。

## AI 生成约束

- 必须优先调用系统 `Notification` 组件。
- 禁止临时创建同类组件。
- 颜色必须来自 `Foundations/tokens.json` 或 `Foundations/tokens.css`。
- 未经 Token 确认的尺寸、圆角、行高不得写死为 Token；需要标记为“待定”或复用项目已有变量。
