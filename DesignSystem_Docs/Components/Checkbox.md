# Checkbox

## 使用场景

- 用于多选或批量选择。

## 允许变体

Checkbox / CheckboxGroup / Indeterminate

## 尺寸与视觉

选中态优先使用品牌色 Token；尺寸：待定。

> 注意：未经 Token 确认的高度、内边距、圆角、行高、阴影均标记为“待定”，不得写成 Token。

## 状态

- default
- checked
- indeterminate
- disabled

## 交互规则

- 表格批量选择必须支持 indeterminate 状态。

## 前端适配

```tsx
<Checkbox checked={checked}>启用</Checkbox>
<CheckboxGroup value={value} options={options} />
```

## 禁止事项

- 禁止多选场景使用多个 Switch 替代。

## AI 生成约束

- 必须优先调用系统 `Checkbox` 组件。
- 禁止临时创建同类组件。
- 颜色必须来自 `Foundations/tokens.json` 或 `Foundations/tokens.css`。
- 未经 Token 确认的尺寸、圆角、行高不得写死为 Token；需要标记为“待定”或复用项目已有变量。
