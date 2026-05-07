# Timeline

## 使用场景

- 用于展示流程记录、审批记录、操作日志。

## 允许变体

Default

## 尺寸与视觉

状态颜色使用状态 Token；尺寸：待定。

> 注意：未经 Token 确认的高度、内边距、圆角、行高、阴影均标记为“待定”，不得写成 Token。

## 状态

- default
- success
- warning
- error

## 交互规则

- 时间、操作人、操作内容必须结构清晰。

## 前端适配

```tsx
<Timeline items={items} />
```

## 禁止事项

- 禁止把 Timeline 做成装饰性页面模块。

## AI 生成约束

- 必须优先调用系统 `Timeline` 组件。
- 禁止临时创建同类组件。
- 颜色必须来自 `Foundations/tokens.json` 或 `Foundations/tokens.css`。
- 未经 Token 确认的尺寸、圆角、行高不得写死为 Token；需要标记为“待定”或复用项目已有变量。
