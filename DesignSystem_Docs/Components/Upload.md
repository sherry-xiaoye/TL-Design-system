# Upload

## 使用场景

- 用于文件上传。

## 允许变体

Button Upload / Drag Upload（待定）

## 尺寸与视觉

尺寸：待定。颜色使用系统 Token。

> 注意：未经 Token 确认的高度、内边距、圆角、行高、阴影均标记为“待定”，不得写成 Token。

## 状态

- default
- uploading
- success
- error
- disabled

## 交互规则

- 必须声明文件类型、大小限制。
- 上传失败必须给出错误提示和重试入口。

## 前端适配

```tsx
<Upload accept=".xlsx,.csv" />
```

## 禁止事项

- 禁止无文件限制说明。
- 禁止上传失败无反馈。

## AI 生成约束

- 必须优先调用系统 `Upload` 组件。
- 禁止临时创建同类组件。
- 颜色必须来自 `Foundations/tokens.json` 或 `Foundations/tokens.css`。
- 未经 Token 确认的尺寸、圆角、行高不得写死为 Token；需要标记为“待定”或复用项目已有变量。
