# Layout

## 标准后台布局

```text
App
├── SideMenu
├── Main
│   ├── Header / PageHeader
│   └── Content
```

## 页面内容结构

页面内容默认由以下模块组成：

1. Breadcrumb：定位当前页面层级。
2. PageHeader：标题、描述、主操作。
3. FilterArea / FormArea / DetailHeader：根据页面类型展示。
4. ContentArea：表格、表单、详情、图表。
5. Pagination / FooterActions：分页或底部操作。

## 布局约束

- 页面背景使用 `--bms-color-bg-page`。
- 内容容器背景使用 `--bms-color-bg-white`。
- 左侧导航背景使用 `--bms-color-bg-menu`。
- 禁止层层嵌套卡片。
- 禁止把后台页面设计成营销页 Hero 布局。

## 待确认

- 顶部栏高度：待定。
- 侧边栏宽度：待定。
- 内容区最大宽度：待定。
