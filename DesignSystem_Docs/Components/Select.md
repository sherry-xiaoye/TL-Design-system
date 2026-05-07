# Select

## 使用场景

- 用于从选项集合中选择单个或多个值。

## 允许变体

Single / Multiple / Searchable（待定）

## 尺寸与视觉

背景使用白色 Token；边框使用表格线 Token；图标使用 `--bms-color-icon-primary-select`；高度、圆角：待定。

> 注意：未经 Token 确认的高度、内边距、圆角、行高、阴影均标记为“待定”，不得写成 Token。

## 状态

- default
- open
- selected
- disabled
- error

## 交互规则

- 选项过多时必须支持搜索。
- 多选项较多时必须处理 tag 溢出。

## 前端适配

```tsx
<Select placeholder="请选择" options={options} />
<Select mode="multiple" options={options} />
```

## 禁止事项

- 禁止用自定义弹层模拟 Select。
- 禁止下拉项无 hover / selected 状态。

## AI 生成约束

- 必须优先调用系统 `Select` 组件。
- 禁止临时创建同类组件。
- 颜色必须来自 `Foundations/tokens.json` 或 `Foundations/tokens.css`。
- 未经 Token 确认的尺寸、圆角、行高不得写死为 Token；需要标记为“待定”或复用项目已有变量。
