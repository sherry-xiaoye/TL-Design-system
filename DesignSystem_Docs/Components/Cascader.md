# Cascader

## 使用场景

- 用于层级数据选择，例如地区、组织、分类。

## 允许变体

Single / Multiple（待定）

## 尺寸与视觉

颜色使用系统 Token；尺寸：待定。

> 注意：未经 Token 确认的高度、内边距、圆角、行高、阴影均标记为“待定”，不得写成 Token。

## 状态

- default
- open
- selected
- disabled
- error

## 交互规则

- 层级选择必须能清晰展示已选路径。

## 前端适配

```tsx
<Cascader options={options} />
```

## 禁止事项

- 禁止用多个 Select 临时拼接复杂层级，除非业务确认。

## AI 生成约束

- 必须优先调用系统 `Cascader` 组件。
- 禁止临时创建同类组件。
- 颜色必须来自 `Foundations/tokens.json` 或 `Foundations/tokens.css`。
- 未经 Token 确认的尺寸、圆角、行高不得写死为 Token；需要标记为“待定”或复用项目已有变量。
