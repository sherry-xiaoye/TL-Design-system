# Table

## 使用场景

- 用于展示结构化数据，是 BMS 核心组件。

## 允许变体

Default / Selectable / Expandable（待定）

## 尺寸与视觉

表头背景 `--bms-color-bg-table-header`；表头文本 `--bms-color-text-table-header`；分割线 `--bms-color-border-table-line`；行高、内边距：待定。

> 注意：未经 Token 确认的高度、内边距、圆角、行高、阴影均标记为“待定”，不得写成 Token。

## 状态

- default
- loading
- empty
- error
- selected
- disabled

## 交互规则

- 必须支持 loading。
- 数据为空必须展示 empty 状态，是否独立 Empty 组件待确认。
- 加载失败必须展示错误提示和重试入口。
- 超长文本必须 ellipsis + Tooltip。
- 操作列保持稳定位置，建议固定右侧。

## 前端适配

```tsx
<Table columns={columns} dataSource={data} loading={loading} emptyText="暂无数据" />
```

## 禁止事项

- 禁止表格无 loading 状态。
- 禁止表格无 empty 状态。
- 禁止操作列按钮换行堆叠。
- 禁止用 div 拼表格。

## AI 生成约束

- 必须优先调用系统 `Table` 组件。
- 禁止临时创建同类组件。
- 颜色必须来自 `Foundations/tokens.json` 或 `Foundations/tokens.css`。
- 未经 Token 确认的尺寸、圆角、行高不得写死为 Token；需要标记为“待定”或复用项目已有变量。
