# Input

## 使用场景

- 用于单行文本、数字、密码等输入。

## 允许变体

Default / Password / Number / Search（待定）

## 尺寸与视觉

背景使用 `--bms-color-bg-white`；边框使用 `--bms-color-border-table-line`；高度、内边距、圆角：待定。

> 注意：未经 Token 确认的高度、内边距、圆角、行高、阴影均标记为“待定”，不得写成 Token。

## 状态

- default
- focus：待定，优先使用品牌色 Token
- disabled
- error
- readonly：待定

## 交互规则

- 必须支持 placeholder。
- 错误提示展示在输入框下方。
- 禁用状态不可聚焦。

## 前端适配

```tsx
<Input placeholder="请输入" />
<Input status="error" />
```

## 禁止事项

- 禁止用 div 模拟输入框。
- 禁止自定义边框颜色。
- 禁止只用红色边框但无错误文案。

## AI 生成约束

- 必须优先调用系统 `Input` 组件。
- 禁止临时创建同类组件。
- 颜色必须来自 `Foundations/tokens.json` 或 `Foundations/tokens.css`。
- 未经 Token 确认的尺寸、圆角、行高不得写死为 Token；需要标记为“待定”或复用项目已有变量。
