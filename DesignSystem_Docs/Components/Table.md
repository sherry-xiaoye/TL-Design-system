# Table

## 1.1 用途

用于结构化数据展示、批量操作、排序、列设置和行内操作。

## 1.2 视觉规范

- 组件：`Table-Header`, `TableHeaderActions`, `Table-Dropdown-Single`, `ColumnSettings`, `Sort`
- Table Header Style：`Default`, `Money`, `Checkbox`, `Empty`, `Action`
- Table Cell State：`Simple`, `Complex`, `Icon`, `Money`, `Checkbox`, `Action`
- 表头背景：`Background/TableHeader`
- 表头文本：`Text/TableHeader`
- 表格线：`Border/Table`
- 最小行高：`40`
- 单元格 padding：`12`

## 1.3 状态规范

- default：正常数据展示。
- hover：行 hover 背景色为`Background/Zebra`。
- loading：必须支持。
- empty：必须支持。

## 1.4 交互规则

- 默认工具栏使用 `TableHeaderActions`。
- 勾选行后切换为批量操作栏，不得同时展示默认工具栏。
- 排序使用 `Sort`。
- 列显示、冻结、宽度配置使用 `ColumnSettings`。
- 行内操作使用 `TextButton` 或 `Link`。

## 1.5 业务场景示例

- 场景 1：【订单列表】中的【查询、筛选、批量导出】。
- 场景 2：【财务报表】中的【列设置、排序、行内编辑】。

## 1.6 前端适配点

- `columns` 映射表头配置。
- `dataSource` 映射接口列表数据。
- `rowSelection` 映射 Checkbox Cell。
- `sorter` 映射 Sort。
- `columnSettings` 映射 ColumnSettings。

## 1.7 AI 生成约束

- 表格必须包含 loading / empty / error 状态。
- 禁止用 div 拼表格。
- 数据量少于等于10条，不使用分页。
- 数据量多于10，禁止省略分页
- 按照业务要求增加复选和批量操作状态。
- 禁止自定义表头颜色和边框。
