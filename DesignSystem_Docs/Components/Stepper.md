# Stepper

## 使用场景

- 用于数值递增递减。

## 允许变体

Default

## 尺寸与视觉

尺寸：待定。颜色使用系统 Token。

> 注意：未经 Token 确认的高度、内边距、圆角、行高、阴影均标记为“待定”，不得写成 Token。

## 状态

- default
- focus
- disabled
- error

## 交互规则

- 必须定义 min / max / step。
- 输入非法值时必须校验。

## 前端适配

```tsx
<Stepper min={0} max={100} step={1} />
```

## 禁止事项

- 禁止无边界的数值输入。

## AI 生成约束

- 必须优先调用系统 `Stepper` 组件。
- 禁止临时创建同类组件。
- 颜色必须来自 `Foundations/tokens.json` 或 `Foundations/tokens.css`。
- 未经 Token 确认的尺寸、圆角、行高不得写死为 Token；需要标记为“待定”或复用项目已有变量。
