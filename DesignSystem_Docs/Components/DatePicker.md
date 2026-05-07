# DatePicker

## 使用场景

- 用于选择日期。

## 允许变体

Date / DateRange

## 尺寸与视觉

边框使用系统边框 Token；高度、内边距、圆角：待定。

> 注意：未经 Token 确认的高度、内边距、圆角、行高、阴影均标记为“待定”，不得写成 Token。

## 状态

- default
- open
- selected
- disabled
- error

## 交互规则

- 日期范围必须明确开始和结束。
- 业务有快捷区间时可提供快捷选择。

## 前端适配

```tsx
<DatePicker />
<DatePicker.RangePicker />
```

## 禁止事项

- 禁止用普通 Input 手写日期格式。

## AI 生成约束

- 必须优先调用系统 `DatePicker` 组件。
- 禁止临时创建同类组件。
- 颜色必须来自 `Foundations/tokens.json` 或 `Foundations/tokens.css`。
- 未经 Token 确认的尺寸、圆角、行高不得写死为 Token；需要标记为“待定”或复用项目已有变量。
