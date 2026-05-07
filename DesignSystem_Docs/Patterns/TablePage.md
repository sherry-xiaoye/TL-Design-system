# TablePage

TablePage 是 BMS 最常见页面模式，用于查询、筛选、列表展示、批量操作和分页。

## 标准结构

```tsx
<Page>
  <Breadcrumb />
  <PageHeader />
  <FilterArea />
  <DataTable />
  <Pagination />
</Page>
```

## 模块顺序

1. Breadcrumb
2. PageHeader
3. FilterArea
4. TableToolbar（如有批量操作）
5. DataTable
6. Pagination

不得随意调整模块顺序。

## FilterArea 规则

- 筛选项横向排列，左对齐。
- 每行最多展示 4 个筛选项，该规则当前为页面契约，具体栅格尺寸待定。
- 查询按钮和重置按钮保持稳定位置，通常位于筛选区尾部。
- 超过 4 个筛选项时，使用“展开 / 收起”高级筛选。
- 筛选区与表格之间间距：待定；如果项目已有 spacing 变量，复用项目变量。
- 筛选组件必须使用系统 Input / Select / DatePicker / Cascader。

## Table 规则

- 表头背景使用 `--bms-color-bg-table-header`。
- 表头文字使用 `--bms-color-text-table-header`。
- 行分割线使用 `--bms-color-border-table-line`。
- 表格行高：待定，未经确认不写成 Token。
- 操作列保持稳定位置，建议固定右侧。
- 超长文本必须使用 ellipsis + Tooltip。
- 空数据必须显示 empty 状态；是否独立 Empty 组件待确认。
- 加载中必须显示 Loading 状态。
- 加载失败必须显示错误提示和重试入口。
- 支持批量选择时，表头 Checkbox 必须支持 indeterminate 状态。

## Pagination 规则

- 分页位于表格下方，通常右对齐。
- 必须包含页码。
- 是否包含每页条数选择：按业务待定。
- 数据量为 0 时不展示分页。

## 状态规则

| 状态 | 规则 |
|---|---|
| loading | 表格区域显示加载状态 |
| empty | 表格区域显示空状态，文案简洁 |
| error | 显示错误提示和重试入口 |
| permission denied | 如无权限，展示权限说明，不展示空表格伪装 |
| disabled | 操作按钮禁用并给出原因，必要时 Tooltip 解释 |

## 禁止事项

- 禁止表格无 loading 状态。
- 禁止表格无 empty 状态。
- 禁止操作列按钮换行堆叠。
- 禁止将筛选区做成多层卡片嵌套。
- 禁止使用营销风 Hero、渐变背景、装饰插画。
- 禁止用 div 拼表格。
- 禁止硬编码非 Token 色值。

## AI 生成约束

- 生成 TablePage 时必须读取 `Components/Table.md`、`Components/Pagination.md`、`Components/Input.md`、`Components/Select.md`。
- 有日期筛选时必须读取 `Components/DatePicker.md`。
- 输出代码后必须按 `Guidelines/AI_Output_Checklist.md` 自检。
