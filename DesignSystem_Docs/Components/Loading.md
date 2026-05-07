# Loading

## 使用场景

- 用于数据加载、表单提交、异步操作等待。

## 允许变体

Page / Block / Inline（待定）

## 尺寸与视觉

颜色优先使用品牌色 Token；尺寸：待定。

> 注意：未经 Token 确认的高度、内边距、圆角、行高、阴影均标记为“待定”，不得写成 Token。

## 状态

- loading

## 交互规则

- 表格加载必须使用 Table 的 loading 状态。
- 提交按钮加载必须使用 Button loading。
- 长时间加载需要可理解文案。

## 前端适配

```tsx
<Loading spinning={loading}>...</Loading>
<Button loading={submitting}>保存</Button>
```

## 禁止事项

- 禁止加载时页面无反馈。
- 禁止重复叠加多个 Loading。

## AI 生成约束

- 必须优先调用系统 `Loading` 组件。
- 禁止临时创建同类组件。
- 颜色必须来自 `Foundations/tokens.json` 或 `Foundations/tokens.css`。
- 未经 Token 确认的尺寸、圆角、行高不得写死为 Token；需要标记为“待定”或复用项目已有变量。
