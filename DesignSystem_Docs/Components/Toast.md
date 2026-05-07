# Toast

## 使用场景

- 用于轻量操作反馈。

## 允许变体

Success / Warning / Error / Info

## 尺寸与视觉

状态颜色使用 Token；位置、尺寸、圆角：待定。

> 注意：未经 Token 确认的高度、内边距、圆角、行高、阴影均标记为“待定”，不得写成 Token。

## 状态

- open
- closed

## 交互规则

- 适合短反馈，例如保存成功、复制成功。
- 重要错误优先使用 Alert 或 Notification。

## 前端适配

```tsx
message.success("保存成功")
```

## 禁止事项

- 禁止用 Toast 承载复杂说明。

## AI 生成约束

- 必须优先调用系统 `Toast` 组件。
- 禁止临时创建同类组件。
- 颜色必须来自 `Foundations/tokens.json` 或 `Foundations/tokens.css`。
- 未经 Token 确认的尺寸、圆角、行高不得写死为 Token；需要标记为“待定”或复用项目已有变量。
